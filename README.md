# k3s-test

export GIT_REPO=https://github.com/boxstep/k3s-test.git
export GIT_TOKEN=

argocd-autopilot repo bootstrap --recover


CA for cert-manager
openssl genrsa -out ca.key 2048
openssl req -new -x509 -key ca.key -out ca.crt
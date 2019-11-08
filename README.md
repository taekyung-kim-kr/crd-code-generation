# crd-code-generation

TL;DR

1. git clone
  - git clone https://github.com/taekyung-kim-kr/code-generator-mod.git
  - git clone https://github.com/taekyung-kim-kr/crd-code-generation.git

2. within code-generator-mod
2.1 ./build.sh
2.2 ./run.sh => OUTPUT should be upper directory of 'crd-code-generation'
2.3 within docker -> /script/codegen.sh crd-code-generation example.com v1

3. within crd-code-generation
3.1 cd artifacts && kubectl apply -f databases-crd.yaml && kubectl apply -f my-database.yaml
3.2 cd cmd/example && go build -o example
3.3 ./example -kubeconfig ./.kube/config

references
1. https://github.com/openshift-evangelists/crd-code-generation
2. https://github.com/kubernetes/apimachinery/issues/63

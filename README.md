# crd-code-generation

TL;DR

1. git clone
    - git clone https://github.com/taekyung-kim-kr/code-generator-mod.git
    - git clone https://github.com/taekyung-kim-kr/crd-code-generation.git

2. within code-generator-mod
    - ./build.sh
    - ./run.sh => OUTPUT should be upper directory of 'crd-code-generation'
    - within docker -> /script/codegen.sh crd-code-generation example.com v1

3. within crd-code-generation
    - cd artifacts && kubectl apply -f databases-crd.yaml && kubectl apply -f my-database.yaml
    - cd cmd/example && go build -o example
    - ./example -kubeconfig ./.kube/config

references
1. https://github.com/openshift-evangelists/crd-code-generation
2. https://github.com/kubernetes/apimachinery/issues/63

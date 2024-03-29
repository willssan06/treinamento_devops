# treinamento_devops

# Devops (Devops + Operações)

## Ferramentas:

- Terraform
- Ansible
- Git e Gitflow
- Docker
- Orquestração de containers
  - Swarmi 
  - Kubernetes 
  - OpenShifit 
- Microserviços
- Monitoramento 
 - Log (Elk, splunk)
 - métricas (Prometheus, zabbix)
- trace
 - Jaeger
 - Datalog
 - dynatrace
- Open xelemetry
- grafana 
- Rundeck 

## Linguagem de script

  - Shell script e power shell
  - Python
  - Ruby Próxima aula 05
  - Go
  - Backups
  - Cron Jobs
  - Monitoramento 

## Linux
- Redes - firewall, servidor de proxy, load balance, protocolo http e https, tcp e udp serviços de redes, IP, DNS, Resolução de nome
- Segurança

## Planejamento 

- scrum (sprints)
- kanban (Backlog esteira)

## Código

- demanda

- desenvolvimento do código

   - versionamento seguindo um git flow e ir para um repositório git remoto (github, gitlab, bitbucket)

## Build (gerar um artefato (pacote de instalação)

   - docker é adotado como padrão para gerar os artefatos)
   - Java -> maven Glade
   - Java script -> npm
   - PHP -> Composer
   - Python -> pip

## Test
   - automatizar testes no pipeline (CI)

## Release

  - processo de liberação de uma nova versão, funcionalidade para o usuário final

  - Deploy (mover a aplicação de um ambiente para outro)

  - código do desenvolvedor -> deploy no ambiente de dev -> deploy no ambiente de hml -> deploy no ambiente de stg -> deploy no ambiente de prod

  - Estratégia de deploy 

    - Rolling (comum em ferramentas de orquestração de containers (Kubernet, OpenShifit)) ambiente 1.0 -> ambiente 2.0 ele aguarda a versão 2,0 estar funcional para cancelar o
      deploy 1.0

    - Blue green ambiente 1.0 -> ambiente 1.0 -> Load balance faz o gerenciamento para qual ambiente deve ser direcionado os usuários

    - canary (feature togglo ou feature flag) (ferramenta HARNESS)ambiente 1.0 -> ambiente 2.0 apenas 10% da base de usuarios fico com a nova versão, com o botão de on e off

## CI / CD (Jenkins, Gitlab, Circle CI, Drone, Harness, Azure Devops)

   - Build -> Test -> release -> deploy (pípeline)

## Preparar a infra (AS CODE)

   - ON premise
   - Cloud 
      - AWS, GCP, AZURE, OCI (ferramentas de provisionamento terraform, gerenciamento de configuração Ansible, Chef, Puppet, Salt)

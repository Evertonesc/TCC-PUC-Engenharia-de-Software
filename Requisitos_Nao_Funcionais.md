# Requisitos Não-Funcionais

A lista a seguir descreve os requisitos não-funcionais do sistema **Orinz**


* O sistema deve ser capaz de processar requisições paralelas e concorrentes com uma taxa de resposta de no máximo 450 ms.

* O sistema, em sua completude, deve estar hospedado em algum provedor de cloud.

* O sistema deverá ter computação elástica para momentos de picos de acesso e momento de baixo tráfego.

* O sistema deve possuir BFF (Back for frontend) para as versão SPA e futuramente para versão Mobile.

* A comunicação com sistemas de integração críticos devem ser feita utilizando o protocolo gRPC

* A autenticação do sistema deve ser assimétrica na geração de tokens JWT e utilizar o algoritmo RSA (Rivest-Shamir-Adleman) na criptografia dos dados do usuário no momento da autenticação

* O sistema _Web_ deve ser responsivo de forma a proporcionar a utilização de qualquer uma de suas funcionalidades em resoluções de 576 _pixels_ até 1080 _pixels_.

* O sistema deve utilizar Mocks para testes de integração, garantindo uma não dependência de integrações externas

* Todo o sistema deve ter no mínimo 70% de cobertura de testes

* Backend, frontend, banco de dados e outros componentes do sistema devem estar rodando em um container docker.
# Criando Readme
Alteração (#1)

Entre na discussão que está aberta e reaja com algum emote e marque presença, vai me ajudar a ganhar conquista no Github.

## Logo agradeço pela compreensão😊

Prompt:

Estou desenvolvendo um SaaS com Java + Spring Boot. Já tenho o backend funcionando com autenticação JWT, cadastro de usuários, cadastro de propriedades e verificação de permissões (admin ou não).

Agora quero transformar minha aplicação em um modelo multi-tenant, onde:
	•	Apenas eu sou o admin global. Nenhum outro usuário pode se registrar como admin.
	•	Cada usuário pode criar uma única empresa (ou grupo), e essa empresa pertence exclusivamente a ele.
	•	As propriedades devem ser vinculadas à empresa do usuário que as cadastrou.
	•	Um usuário só pode ver e cadastrar propriedades da sua própria empresa.
	•	Preciso impedir que um mesmo usuário crie mais de uma empresa, para evitar ocupar demais o banco gratuito da Render.

O que eu preciso:
	1.	As entidades JPA necessárias (User, Empresa, Propriedade) com os relacionamentos corretos.
	2.	Os repositórios com os métodos apropriados.
	3.	Os serviços com as regras de negócio (como impedir múltiplas empresas por usuário e vincular propriedade à empresa do usuário logado).
	4.	Exemplos de controladores REST para criar empresa, cadastrar propriedade e listar as propriedades da empresa do usuário logado.

Já tenho autenticação funcionando com token JWT. O ID do usuário logado está acessível via SecurityContextHolder.

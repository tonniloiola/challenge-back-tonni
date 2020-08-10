### Desafio

Criar uma API (Rest/Restful) para gestão de usuários, que terão dois perfis de acesso: ADMINISTRADOR e VISITANTE.
Utilizaremos o cadastro do usuário para realizar a autenticação (login) e autorização (restringir endpoints). 

### Requisitos
- Criar uma api para gestão (CRUD) de usuários onde seja possível
    - Cadastrar um novo usuário (endpoint público);
    - Ler um usuário cadastrado a partir do seu ID (endpoint restrito ao perfil ADMINISTRADOR ou o próprio usuário);
    - Listar usuários cadastrados (endpoint restrito ao perfil ADMINISTRADOR);
    - Atualizar usuário (endpoint restrito ao perfil ADMINISTRADOR ou o próprio usuário);
- Criar na api um endpoint para o usuário poder logar-se informando o usuário e senha (endpoint público);
- Criar na api um endpoint para o usuário poder deslogar-se (endpoint público);
- O login do usuáro deve ser por e-mail, sende esse único na base de daos;
- O login deverá retornar um token para que a comunicação de usuário logado seja feita;

### Requisitos não fucionais

- Os dados deverão ser armazenados em banco de dados relacional (postgres, mysql, etc);
- Ulitzar Java 11+;
- Utilizar um framework web atual: Spring-boot

###Utilização
Mysql rodando com docker, comando para subir o docker
- docker-compose -f "stack.yml" up -d

Existe dois usuarios cadastrados para teste:
-   usuario: admin@gmail senha: 1  com perfil Administrador
-   usuario: user@gmail senha: 1  com perfil Usuario

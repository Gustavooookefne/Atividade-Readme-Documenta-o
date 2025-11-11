# 📋 Gerenciamento de Tarefas (SESI)

Este projeto é uma aplicação de gerenciamento de tarefas simples desenvolvida com Spring Boot e Spring Data JPA, seguindo o padrão MVC (Model-View-Controller). Ele permite o registro, visualização, edição e exclusão de Usuários, Categorias de Tarefas e Tarefas associadas.

# 🛠️ Tecnologias Utilizadas
- *Linguagem:* Java
- *Framework:* Spring Boot
- *Persistência:* Spring Data JPA
- *Banco de Dados:* (Presume-se um DB configurado no application.properties, como H2, MySQL, PostgreSQL, etc.)
- *Frontend/View:* (Presume-se o uso de uma tecnologia de templates como Thymeleaf ou JSP para as views referenciadas nos Controllers: listarTarefaCategoria, formularioTarefaCategoria, listarTarefas, formularioTarefa, listarUsuarios, formularioUsuario).

# 🏗️ Estrutura do Projeto


# 🚀 Como Executar o Projeto

- Clone o Repositório: Obtenha o código-fonte do projeto.
- Configuração do Banco de Dados: Certifique-se de que as configurações de conexão com o banco de dados estão corretas no arquivo application.properties (ou similar).
- Compilação: Compile o projeto (ex: usando Maven ou Gradle).
- Configuração do Banco de Dados: Certifique-se de que as configurações de conexão com o banco de dados estão corretas no arquivo application.properties (ou similar).
- Compilação: Compile o projeto (ex: usando Maven ou Gradle).
- Execução: Execute a classe principal do Spring Boot (com.sesi.tarefas.TarefasApplication - nome presumido). A classe CarregaBaseDeDados garantirá que os dados iniciais sejam carregados.
- Acesso: O aplicativo estará acessível na porta configurada (geralmente http://localhost:8080).

# 🔑 Rotas Principais (Endpoints)
Funcionalidade&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Endpoint (GET) <br>
Listar Categorias&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;listarCategoria <br>
Listar Usuários&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usuarios/listarUsuarios <br>
Listar Tarefas&emsp;&emsp;&emsp; &emsp; &emsp;&emsp;&emsp; tarefas/listarTarefas <br>
Formulário Nova Tarefa&emsp;&emsp;&emsp; tarefas/novo <br>


# 🏗️ Estrutura do Projeto

mn-gerenciador-tarefas/
 ├── src<br>
 │   ├── main<br>
 │ &ensp;  │ &ensp;  ├── java<br>
 │ &ensp;  │ &ensp;  │   └── com.sesi.tarefas<br>
 │ &ensp;  │ &ensp;  │  &ensp;     ├── config<br>
 │ &ensp;  │ &ensp;  │  &ensp;     │   └── DataLoader.java<br>
 │ &ensp;  │ &ensp;  │   &ensp;    ├── controller<br>
 │ &ensp;  │ &ensp;  │  &ensp;    │   ├── TarefaController.java<br>
 │ &ensp;  │ &ensp;  │       │   ├── UsuarioController.java<br>
 │ &ensp;  │ &ensp;  │       │   └── TarefaCategoriaController.java<br>
 │ &ensp;  │ &ensp;  │       ├── model<br>
 │ &ensp;  │ &ensp;  │       │   ├── Tarefa.java<br>
 │ &ensp;  │ &ensp;  │       │   ├── Usuario.java<br>
 │ &ensp;  │ &ensp;  │       │   ├── TarefaCategoria.java<br>
 │ &ensp;  │ &ensp;  │       │   ├── StatusTarefa.java<br>
 │ &ensp;  │ &ensp;  │       │   └── Prioridade.java<br>
 │ &ensp;  │ &ensp;  │       └── repository<br>
 │ &ensp;  │ &ensp;  │           ├── TarefaRepository.java<br>
 │ &ensp;  │ &ensp;  │           ├── UsuarioRepository.java<br>
 │ &ensp;  │ &ensp;  │           └── TarefaCategoriaRepository.java<br>
 │ &ensp;  │ &ensp;  └── resources<br>
 │ &ensp;  │ &ensp;      ├── application.yml<br>
 │ &ensp;  │ &ensp;      └── logback.xml<br>
 │ &ensp;  └── test<br>
 │ &ensp;      └── java<br>
 │ &ensp;          └── com.sesi.tarefas<br>
 │ &ensp;              └── GerenciadorTarefasTest.java<br>
 ├── build.gradle  (ou pom.xml)<br>
 └── README.md



<div align='center'>

# Gestor de Tarefas com Laravel

</div>

**O projeto foi feito seguindo o passo-a-passo da criação do mesmo, no curso Desenvolvimento Web Compacto e Completo de João Ribeiro na Udemy, no módulo de Laravel do curso.**

**Ao longo do desenvolvimento do sistema, notei um erro na parte das views de editar e excluir task. Notei que estavam sendo apresentadas as tasks que haviam sido excluídas, pois estava faltando o termo `->whereNull('deleted_at')` nessas chamadas das tasks.**

**Então pude contribuir informando ao professor sobre esse erro. Também pude aprender mais sobre Laravel e suas funcionalidades, bem como a utilizar Datatables e o Bootstrap junto do Laravel.**

## Tecnologias Utilizadas

<div align='center'>

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) ![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white) ![html](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) ![css](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white) ![Javascript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E) ![Mysql](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white) ![Dbeaver](https://img.shields.io/badge/dbeaver-382923?style=for-the-badge&logo=dbeaver&logoColor=white)

</div>

## Funcionalidades

- **Login de Usuários, onde foi criado dois Middlewares para checar se o usuário está logado ou não.**
- **CRUD de Tasks, com softdelete e validação dos inputs dos formulários.**
- **O frontend foi feito utilizando o Bootstrap 5 junto com o Blade.**
- **Na listagem de tasks, a tabela foi criada com DataTables, onde foi preciso mexer um pouco no Jquery para apresentar os dados.**
- **Ainda na listagem das tasks, foi criada uma caixa de pesquisa de task e um um filtro de task, que filtra as tasks pelo Status.**

## Como rodar o projeto

1. **Conecte seu banco através do arquivo .env(use o .env.example e crie seu .env)**
2. **`php artisan migrate` para rodar as migrations e criar as tabelas de users e tasks.**
3. **`php artisan db:seed --class=UsersSeeder` para popular a tabela users, com três usuários (user1, user2 e user3), a senha é o mesmo nome do usuário (user1, user2 e user3).**
4. **`php artisan serve` para rodar um servidor local de teste.**
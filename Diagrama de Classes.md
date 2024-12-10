## Diagrama de Classes

![Diagrama de Classe](https://github.com/tads-cnat/MipsCode/blob/main/doc/dominio/Classes.JPG)

## Modelo Relacional

![Diagrama ER Relacional](https://github.com/tads-cnat/MipsCode/blob/main/doc/doc-ORM/Relacional.JPG)


## Classes versus Tabelas
| Classe              |  Tabela             |   Significado       |
| :-----------------: | :-----------------: | :-----------------: |
| User                | User                |  Modelo de login padrão do django. | 
| Profile             | Profile             | Classe que representa o perfil do usuário que armazena project e tutorials. |
| Documentation       | Documentation       | Classe que armazena a aba de “documentação” do site. |
| Project             | Project             | Classe que representa os projetos do usuário. |
| Tutorial            | Tutorial            | Classe que representa a aba de tutoriais do site. |


## Relacionamentos
| Tabela Origem       |  Through            |   Tabela Destino    | Significado         |
| :-----------------: | :-----------------: | :-----------------: | :-----------------: |
| Profile             |  -                  |  User               | Indica o login que criou o perfil. |
| Tutorial            |  -                  |  Profile            | Indica o Perfil que criou o tutorial. |
| Project             |  -                  |  Profile            | Indica o Perfil que criou o projeto. |

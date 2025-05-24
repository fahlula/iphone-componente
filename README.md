# Desafio de Modelagem e Diagramação - Componente iPhone

Descrição
Este projeto representa a modelagem UML do componente **iPhone** inspirado no vídeo de lançamento original de 2007. O iPhone foi modelado com três funcionalidades principais:

- Reprodutor Musical  
- Aparelho Telefônico  
- Navegador de Internet

## 📐 Diagrama UML

Você pode visualizar o diagrama UML neste link:
[https://www.mermaidchart.com/app/projects/8d7688cb-75f3-4cac-ba4e-542b92bb0d66/diagrams/de80fa61-dbba-46a9-9323-48e193b6ea06/version/v0.1/edit](https://www.mermaidchart.com/app/projects/8d7688cb-75f3-4cac-ba4e-542b92bb0d66/diagrams/de80fa61-dbba-46a9-9323-48e193b6ea06/version/v0.1/edit)

### Exemplo de Diagrama UML (Mermaid)
```mermaid
classDiagram
    class ReprodutorMusical {
        <<interface>>
        +tocar()
        +pausar()
        +selecionarMusica(musica: String)
    }

    class AparelhoTelefonico {
        <<interface>>
        +ligar(numero: String)
        +atender()
        +iniciarCorreioVoz()
    }

    class NavegadorInternet {
        <<interface>>
        +exibirPagina(url: String)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class IPhone {
        +tocar()
        +pausar()
        +selecionarMusica(musica: String)
        +ligar(numero: String)
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina(url: String)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    ReprodutorMusical <|.. IPhone
    AparelhoTelefonico <|.. IPhone
    NavegadorInternet <|.. IPhone
```



Linguagem Utilizada
Java (para implementação das interfaces e classe)

/iphone-componente
├── README.md
├── ReprodutorMusical.java
├── AparelhoTelefonico.java
├── NavegadorInternet.java
└── IPhone.java


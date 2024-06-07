# Desafio UML iPhone

Projeto do curso DIO para modelar e implementar as funcionalidades do iPhone de 2007 usando UML e Java. Funcionalidades incluem Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

- **Reprodutor Musical**: tocar(), pausar(), selecionarMusica(String musica)
- **Aparelho Telefônico**: ligar(String numero), atender(), iniciarCorreioVoz()
- **Navegador na Internet**: exibirPagina(String url), adicionarNovaAba(), atualizarPagina()

## Diagrama UML

```mermaid
classDiagram
    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    
    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    
    class NavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    
    class iPhone {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    
    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet

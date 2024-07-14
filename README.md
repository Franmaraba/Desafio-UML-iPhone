# Desafio-UML-iPhone
Criando desafio de Modelagem e Diagramação de um Componente iPhone

## autor 
[Francisco Rodrigues](https://github.com/Franmaraba)


```mermaid
classDiagram
    
    class ReprodutorMusical{
        <<interface>>
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
      
    }
    class AparelhoTelefonico{
      <<interface>>
      +ligar(String numero)
      +atender()
      +iniciarCorreioVoz()
    }
    class NavegadorInternet{
        <<interface>>
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
      
    }
    class Ipod{

    }
    class Smartphone{

    }
    class Mac{

    }
    class Iphone{
        
    }


    ReprodutorMusical <|-- Iphone 
    AparelhoTelefonico <|-- Iphone
    NavegadorInternet <|-- Iphone
    ReprodutorMusical <|-- Ipod
    AparelhoTelefonico <|-- Smartphone
    NavegadorInternet <|-- Mac

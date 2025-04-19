# 🚀 Desafio DIO: Modelagem UML do iPhone 2007

## 🎯 Objetivo do Projeto

Este projeto visa capturar a essência inovadora do primeiro iPhone através de uma representação UML precisa, inspirada diretamente no marco histórico de seu lançamento. O diagrama reflete as três revoluções tecnológicas que Steve Jobs apresentou ao mundo em 9 de janeiro de 2007.


## 🔍 Visão Geral do Diagrama  
Este projeto modela três componentes principais do iPhone:  

1. **🎵 Reprodutor Musical** – Controle de músicas e playlists.  
2. **📞 Aparelho Telefônico** – Gestão de chamadas e contatos.  
3. **🌐 Navegador na Internet** – Navegação web e histórico.  

## 💬 Citação Emblemática

> "Não são três dispositivos separados - é um único dispositivo. E nós o chamamos de iPhone."  
> **Steve Jobs, Macworld 2007**



## 📊 Diagrama UML  

```mermaid
classDiagram
    class Phone {
        <<interface>>
    }

    class ReprodutorMusical {
        +selecionarMusica(musica: String)
        +tocar()
        +pausar()
        +ajustarVolume(nivel: int)
        +avancarMusica()
        +retrocederMusica()
        +exibirPlaylist(): List
    }

    class AparelhoTelefonico {
        +ligar(numero: String)
        +atender()
        +iniciarCorreioVoz()
        +encerrarChamada()
        +adicionarContato(nome: String, numero: String)
        +bloquearNumero(numero: String)
        +visualizarHistoricoChamadas(): List
    }

    class NavegadorInternet {
        +exibirPagina(url: String)
        +adicionarNovaAba()
        +atualizarPagina()
        +fecharAba()
        +exibirFavoritos(): List
        +adicionarAosFavoritos(url: String)
        +limparHistorico()
    }

    Phone <|-- ReprodutorMusical
    Phone <|-- AparelhoTelefonico
    Phone <|-- NavegadorInternet
```
## ▶️ Vídeo Referência que inspirou esse Projeto
- [[Steve Jobs apresenta o iPhone]](https://www.youtube.com/watch?v=9ou608QQRq8 "Assistir ao lançamento completo")

## 📚 Ferramenta Utilizada
- [[Mermaid]](https://www.mermaidchart.com/app/projects)



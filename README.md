# 📱 iPhone UML Diagram - Reprodutor Musical, Aparelho Telefônico e Navegador na Internet  

Um diagrama UML moderno que representa as funcionalidades essenciais do **iPhone** inspirado no lançamento de 2007!  

---

## 🔍 Visão Geral do Diagrama  
Este projeto modela três componentes principais do iPhone:  

1. **🎵 Reprodutor Musical** – Controle de músicas e playlists.  
2. **📞 Aparelho Telefônico** – Gestão de chamadas e contatos.  
3. **🌐 Navegador na Internet** – Navegação web e histórico.  

---

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
## Vídeo Referência que inspirou esse Projeto
[![Steve Jobs apresenta o iPhone]](https://www.youtube.com/watch?v=9ou608QQRq8 "Assistir ao lançamento completo")

## 📚 Recursos Úteis
- [Mermaid.js Documentation](https://mermaid.js.org/) - Guia completo de sintaxe e exemplos



# 📺 API TV - Sistema de Streaming & Postagem

O **API TV** é uma plataforma web para agregação de conteúdo audiovisual, permitindo a reprodução de listas M3U8, canais do YouTube e vídeos diretos (MP4/MKV). O sistema conta com um painel de postagem colaborativa onde usuários autorizados podem publicar seus próprios filmes.

---

## 🚀 Funcionalidades Principais

* **Multiformatos:** Suporte nativo para links `.m3u8`, `.mp4`, `.mkv` e integração total com **YouTube** e **Twitch**.
* **Painel de Postagem:** Área restrita para criadores publicarem conteúdos na aba "POST FILMES GRÁTIS".
* **Perfis Personalizados:** Cada autor pode definir seu **nome de exibição** e **imagem de perfil**, que aparecem automaticamente em cada postagem.
* **Gestão via Nuvem:** Integração em tempo real com **Firebase Realtime Database** para sincronização de listas e usuários.
* **Interface Gamer/LED:** Design responsivo otimizado para dispositivos móveis com efeitos de iluminação dinâmica.

---

## 🛠️ Tecnologias Utilizadas

* **Frontend:** HTML5, CSS3 (Variáveis Modernas & Flexbox/Grid), JavaScript (Vanilla).
* **Player:** [Clappr](https://github.com/clappr/clappr) para HLS e reprodução de vídeo.
* **Banco de Dados:** Firebase Realtime Database para armazenamento de conteúdos e metadados de usuários.
* **Streaming:** Integração com APIs da Twitch e Embeds do YouTube.

---

## 📁 Estrutura do Banco de Dados (Firebase)

O sistema organiza os dados da seguinte forma:

| Caminho | Descrição |
| :--- | :--- |
| `/listas` | Armazena as URLs das listas M3U principais. |
| `/youtube` | Armazena os filmes e canais postados (incluindo dados do autor). |
| `/usuarios_premium` | Gerencia os IDs de acesso, nomes e fotos de perfil dos postadores. |
| `/visual` | Armazena a configuração de imagem de fundo do cabeçalho. |

---

## 🔑 Como Utilizar o Painel de Postagem

1.  **Solicitar Acesso:** No menu **POST FILMES**, clique em "Solicitar Acesso". Um ID único será gerado e enviado via WhatsApp para validação.
2.  **Configurar Perfil:** Após logar com seu ID, você pode definir o nome do seu canal e o link da sua foto de perfil.
3.  **Publicar:** Insira o nome do filme, o link da capa (poster) e a URL do vídeo. Ao clicar em **Postar Agora**, seu conteúdo aparecerá instantaneamente para todos os usuários na categoria "Reve Filmes".

---

## 📝 Notas de Versão

* **v2.0:** Mudança de nome para *API TV*, adição de sistema de foto de perfil para autores e otimização de renderização de grid.
* **v1.5:** Implementação do modo Tela Cheia e integração com canais ao vivo da Twitch.

---
Desenvolvido para proporcionar uma experiência fluida de IPTV e Cinema Web.

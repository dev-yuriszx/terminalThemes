# 🖥️ Terminal Themes

Um script em Bash para personalizar o terminal Linux com **prompts (PS1)** e  **imagens de fundo** , com menu interativo via `fzf` e integração com o terminal entity["software","Kitty","terminal emulator"].

Ideal para quem gosta de deixar o terminal com uma aparência mais personalizada sem precisar editar arquivos manualmente.

---

## ✨ Funcionalidades

* Alterar o prompt do terminal (PS1) por menu interativo
* Alterar imagem de fundo do terminal
* Aplicar prompt + background em conjunto (modo combo)
* Restaurar o último tema automaticamente ao abrir o terminal
* Resetar tudo para o padrão
* Adicionar novas imagens de fundo
* Remover imagens e restaurá-las da lixeira interna

---

## 📦 Dependências

Antes de usar, o projeto utiliza:

* entity["software","fzf","command-line fuzzy finder"] — menu interativo no terminal
* entity["software","Kitty","terminal emulator"] — para suporte a imagens de fundo
* Bash
* Linux (testado em distribuições baseadas em Debian/Ubuntu)

---

## 🚀 Instalação

Clone o repositório:

```bash
git clone https://github.com/yuri-xyzs/terminalThemes
cd terminalThemes
chmod +x terminal_theme_install
./terminal_theme_install
```

Após instalar:

```bash
source ~/.bashrc
```

Depois, rode:

```bash
theme
```

---

## 📂 Estrutura do projeto

```bash
.terminalThemes/
├── backgrounds/
│   └── imgs/
├── PS1s/
├── terminal_theme_bot
├── terminal_theme_functions
├── terminal_get_theme
└── .my_last_theme
```

---

## 🧩 Como funciona

### `terminal_theme_bot`

Script principal com menu interativo. Permite selecionar:

* alterar prompt
* alterar background
* resetar tudo
* aplicar combo
* adicionar/remover imagens

### `terminal_theme_functions`

Arquivo com todas as funções auxiliares:

* aplicar tema
* salvar último tema usado
* resetar configurações
* restaurar imagens removidas

### `terminal_get_theme`

Executado automaticamente ao abrir o terminal para reaplicar o último tema salvo.

---

## 🛠 Comando principal

Após instalação, o projeto adiciona este comando ao `.bashrc`:

```bash
theme
```

Ele abre o menu visual para gerenciar os temas.

---

## 💡 Exemplo

Ao rodar:

```bash
theme
```

Você verá opções como:

```text
✞ Alterar prompt
✞ Alterar background img
✞ Reset all
✞ Combo!!!
✞ adicionar / remover bk_img
```

---

## 🔥 Destaques técnicos

Este projeto utiliza:

* Bash scripting
* manipulação de arquivos
* persistência via arquivo oculto (`.my_last_theme`)
* integração com terminal gráfico
* menus interativos com fzf
* automação de configuração do `.bashrc`

---

## 📌 Observações

* O fundo com imagem funciona apenas no entity["software","Kitty","terminal emulator"].
* Se estiver usando outro terminal, apenas o prompt será alterado.
* O script salva automaticamente a última configuração utilizada.

---

## 👨‍💻 Autor

Desenvolvido por Yuri Barroso.

Se quiser contribuir ou sugerir novos temas, fique à vontade para abrir um pull request.

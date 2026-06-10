# ♻️ Recicla Vizinho

Bem-vindo ao **Recicla Vizinho**! Este é um projeto universitário desenvolvido por estudantes de Tecnologia, com o objetivo de promover a conscientização ambiental, o senso de comunidade e facilitar a denúncia de descarte irregular de lixo e entulho nos bairros.

## 🚀 Como Rodar o Projeto Localmente

Para garantir que todas as funcionalidades do site operem corretamente (especialmente o envio de formulários e redirecionamentos), o projeto **deve** ser executado através de um servidor local. 

Recomendamos o uso da extensão **Live Server** no Visual Studio Code:

1. Abra a pasta principal do projeto (`Recicla_Vizinho-main`) no VS Code.
2. Certifique-se de ter a extensão **[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)** instalada.
3. No explorador de arquivos lateral, clique com o botão direito sobre o arquivo principal: `index.html`.
4. Selecione a opção **"Open with Live Server"** (ou use o atalho `Alt + L, Alt + O`).
5. O navegador será aberto automaticamente na URL local (ex: `http://127.0.0.1:5500/index.html`). A partir daí, você pode navegar por todas as telas do projeto.

---

## 📢 Sistema de Denúncias (Funcional)

A principal funcionalidade da plataforma é a tela de **Denúncia**, que está 100% funcional e integrada à API do FormSubmit para o envio de e-mails, suportando inclusive o anexo de imagens.

### Como testar o fluxo de envio:
O sistema foi desenhado para proteger os dados do usuário e evitar spam, seguindo este fluxo:

1. Desça até a parte de **Denúncia** (ou clique no botão na página inicial).
2. Preencha os dados do local e a descrição do problema (o nome do denunciante é **opcional** para garantir o anonimato). Você também pode anexar uma foto do local.
3. Clique em **Enviar denúncia**.
4. **Validação de Segurança:** Uma **nova aba** será aberta automaticamente no seu navegador com um desafio Captcha (verificação de "Não sou um robô"). 
5. **Retorno:** Após concluir o Captcha na nova aba, basta fechá-la. Ao voltar para a tela do nosso site, você verá um **Popup de Sucesso** confirmando o processo, e os campos do formulário já estarão limpos para uma nova denúncia.
6. **Confirmação Automática:** O e-mail preenchido no formulário receberá uma mensagem automática de confirmação de recebimento (verifique a caixa de Spam).

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estruturação semântica de todas as páginas.
* **CSS3:** Estilização, layout flexível e design responsivo.
* **JavaScript:** Controle de interface (DOM) para exibição de modais de sucesso e limpeza dinâmica de formulários.
* **FormSubmit API:** Integração *front-end* para roteamento seguro de e-mails e anexos (arquitetura *serverless*).

---

## 👥 Equipe Desenvolvedora
*Projeto desenvolvido por um grupo de três estudantes de Tecnologia focado em soluções para comunidades sustentáveis.*
### Página de Login

<b>Funcionalidade:</b>
Entrar ou Cadastrar-se no site


<b>Contexto:</b>
    Dado que usuário não possui cadastro no sistema

<b>Cenário:</b> Cadastro de conta
    E usuário preenche todas as informações do formulário obrigatórias corretamente
Quando aciona a opção de "Cadastrar"
Então obtém sua conta
E é redirecionado para a área de Login


<b>Contexto:</b>
    Dado que o usuário possui cadastro no sistema

<b>Cenário:</b> Login válido  
    E usuário preenche o formulário com credenciais válidas
Quando ele aciona a opção "Entrar"
Então é redirecionado para a página Home

<b>Cenário:</b> Login com credenciais incorretas
    E o usuário preenche o formulário com credencias inválidas
Quando ele aciona a opção "Entrar"
Então deve ser exibida uma mensagem "Email ou senha inválidos" 
E o usuário deve preencher as credenciais novamente

<b>Cenário:</b> Usuário esqueceu sua senha
    E o usuário preenche o formulário com a senha incorreta
Quando ele aciona a opção "Entrar"
Então deve ser exibida uma mensagem "Senha incorreta"
Quando o usuário acionar a opção "Esqueci minha senha"
Então o usuário pode criar uma nova senha 
E é redirecionado para a área de login

### Página de Contato

<b>Funcionalidade:</b> Entrar em Contato

<b>Contexto:</b>
    Dado que o usuário está preenchendo o formulário.

<b>Cenário:</b> Contato válido
    E usuário preenche todos os campos
Quando ele aciona o botão "enviar"
Então nos envia uma mensagem. 

<b>Cenário:</b> Contato inválido
    E usuário deixou um o mais campos vazios
Quando ele aciona o botão "enviar" 
Então deve ser exibida uma mensagem "Preencha o campo vazio"
    
### Página de Assalto

<b>Funcionalidade:</b> Registrar um Assalto

<b>Contexto:</b> 
    Dado que o usuário está logado
E tenta registrar um assalto

<b>Cenário:</b> Assalto registrado com sucesso
    E usuário aciona o botão "Registrar Assalto"
E usuário preenche todos os campos
Quando ele aciona o botão "registrar"
Então o assalto é registrado com êxito 
E exibe uma mensagem "Assalto Registrado."
    
<b>Cenário:</b> Assalto não registrado
    E usuário aciona o botão "Registrar Assalto"
E usuário não preenche todos os campos corretamente 
Quando ele aciona o botão "Registrar"
Então exibe uma mensagem "Preencha os campos corretamente"
    
<b>Contexto:</b>
    Dado que o usuário não está logado
E tenta registrar um assalto
    
<b>Cenário:</b> Assalto não registrado
    E usuário aciona o botão "Registrar Assalto"
Então exibe uma mensagem "É preciso estar logado"
E é redirecionado para a área de Login/Cadastro
    
    




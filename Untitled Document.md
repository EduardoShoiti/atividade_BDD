### Página de Login

Funcionalidade: 
Entrar ou Cadastrar-se no site

Contexto: 
Dado que usuário não possui cadastro no sistema

Cenário: Cadastro de conta
E usuário preenche todas as informações do formulário obrigatórias corretamente
Quando aciona a opção de "Cadastrar"
Então obtem sua conta
E é redirecionado para a área de Login


Contexto:
Dado que o usuário possui cadastro no sistema

Cenário: Login válido  
E usuário preenche o formulário com credenciais válidas
Quando ele aciona a opção "Entrar"
Então é redirecionado para a página Home

Cenário: Login com credenciais incorretas
E o usuário preenche o formulário com credencias inválidas
Quando ele aciona a opção "Entrar"
Então deve ser exibida uma mensagem "Email ou senha incorreta" 
E o usuário deve preencher as credenciais novamente

Cenário: Usuário esqueceu sua senha
E o usuário preenche o forumlário com a senha incorreta
Quando ele aciona a opção "Entrar"
Então deve ser exibida uma mensagem "Senha incorreta"
Quando o usuário acionar a opção "Esqueci minha senha"
Então o usuário pode criar uma nova senha 
E é redirecionado para a área de login





# Guia de Acesso Internet

Este guia mostra como configurar e obter acesso à VPN usando o FortiClient.

## Pré-requisitos

- **FortiClient**: Certifique-se de que você tenha o FortiClient instalado no seu dispositivo. Você pode baixá-lo nos links abaixo:
  - [Download para Windows](https://www.fortinet.com/products/endpoint-security/forticlient)
  - [Download para macOS](https://www.fortinet.com/products/endpoint-security/forticlient)

- **Credenciais VPN**: Solicite ao administrador de rede o endereço do servidor VPN, seu nome de usuário e senha.

## Passo a Passo

### 1. Instalar o FortiClient

1. Acesse o [site oficial do FortiClient](https://www.fortinet.com/products/endpoint-security/forticlient) e baixe a versão para o seu sistema operacional.
2. Instale o FortiClient seguindo as instruções no instalador.

### 2. Configurando o FortiClient

1. Abra o **FortiClient** após a instalação.
2. No painel inicial, selecione a opção **Remote Access**.
3. Clique em **Configure VPN**.

### 3. Adicionando a VPN

1. Preencha os campos com as informações fornecidas pelo administrador de rede:
    - **VPN Type**: Escolha **SSL-VPN**.
    - **Remote Gateway**: Insira o endereço do servidor VPN (ex: `vpn.empresa.com`).
    - **Port**: Normalmente, o FortiClient utiliza a porta `443` para SSL-VPN.
    - **Authentication**:
      - **Username**: Seu nome de usuário.
      - **Password**: Sua senha.
    - **Client Certificate**: Deixe como **None**, a menos que seja instruído a usar um certificado específico.

2. Marque a opção **Save login** se desejar salvar suas credenciais.
3. Clique em **Save** para salvar a configuração da VPN.

### 4. Conectando à VPN

1. No painel do FortiClient, vá até **Remote Access** e selecione a VPN que você acabou de configurar.
2. Clique em **Connect**.
3. Insira suas credenciais se solicitado, e clique em **OK**.
4. Quando conectado, a interface do FortiClient mostrará o status **Connected**.

### 5. Desconectando da VPN

- Para desconectar, volte ao painel do FortiClient e clique em **Disconnect**.

## Solução de Problemas

- Se você não conseguir se conectar, verifique:
  - Se o endereço do servidor VPN está correto.
  - Se você está conectado à internet.
  - Se suas credenciais estão corretas.
  - Se o FortiClient está atualizado para a versão mais recente.

Para mais assistência, entre em contato com o administrador da rede.

---

**Aviso**: O acesso VPN é restrito e monitorado pela equipe de TI. Certifique-se de seguir as políticas de segurança da sua empresa.

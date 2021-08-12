<!-- markdownlint-disable MD002 MD041 -->

Antes de usar o Microsoft Graph Data Connect pela primeira vez, você precisa configurar seu locatário do Microsoft 365. Isso envolve a adição do serviço e a configuração de um grupo de segurança com permissões para aprovar solicitações de extração de dados.

## <a name="grant-azure-ad-users-the-global-administrator-role"></a>Conceder aos usuários do Azure AD a função de administrador global

Nesta etapa, você garantirá que dois usuários no locatário do Microsoft 365 tenham a **função de** administrador global habilitada.

- [Função de administrador global integrado](/azure/active-directory/roles/permissions-reference#global-administrator).
- [Elevar o acesso para obter a função administrador global](/azure/role-based-access-control/elevate-access-global-admin).

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a>Configurar o grupo aprovador de solicitação de consentimento do Microsoft Graph Data Connect

Nesta etapa, você configurará seu locatário do Microsoft 365 para habilitar o uso do Microsoft Graph Data Connect.

1. Abra um navegador e vá para o Portal de Administração do [Microsoft 365.](https://admin.microsoft.com/)

1. Na navegação da barra lateral, selecione **Grupos ativos**.
  
    ![Uma captura de tela mostrando os grupos ativos no Centro de administração do Microsoft 365.](images/data-connect-m365-act-grp.png)

1. Selecione o **botão Adicionar um grupo.**

1. Use o seguinte para criar o novo grupo de segurança habilitado para **email** e selecione o **botão Adicionar.**
   - **Tipo**: segurança habilitada para email

    ![Uma captura de tela mostrando um usuário selecionando a segurança habilitada para email para um novo grupo no centro de administração do Microsoft 365.](images/data-connect-m365-mail-sec.png)

   - **Nome**: Aprovadores de Solicitação de Consentimento

    ![Uma captura de tela mostrando um usuário está dando ao grupo um nome de "Aprovadores de Solicitação de Consentimento" no Centro de administração do Microsoft 365.](images/data-connect-m365-cons-apprv.png)

   - **Prefixo de Email**: consentrequestapprovers

    ![Uma captura de tela mostrando um usuário criando o endereço de email do grupo criado anteriormente no centro de administração do Microsoft 365.](images/data-connect-m365-cons-apprv-pref.png)

1. **Pode levar até uma hora até** o grupo recém-criado aparecer na lista. Quando o grupo tiver sido criado, selecione-o.

1. Vá para a **opção Grupos ativos** novamente e procure o grupo que você acabou de criar.

1. Selecione o grupo e, na guia **Membros,** selecione **Exibir tudo e gerenciar membros**.

1. Adicione os dois usuários que você habilitaram a **função de** administrador global a esse novo grupo.

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a>Habilitar o Microsoft Graph Data Connect no locatário do Microsoft 365

Nesta etapa, você habilita o serviço Microsoft Graph Data Connect em seu locatário do Microsoft 365.

1. Enquanto você ainda estiver inscreveu no Portal de Administração do Microsoft 365, selecione o item de menu **Configurações > Org.**

1. Selecione o **serviço Microsoft Graph Data Connect.**

    ![Uma captura de tela mostrando o "Serviços" na folha "Configurações da organização". Um usuário está toggling on the Microsoft Graph Data Connect service in the Microsoft 365 admin center.](images/data-connect-m365-mgdc-toggle.png)

1. Selecione a caixa de seleção que diz ativar ou desativar o **Microsoft Graph Data Connect para que toda a** sua organização habilita a Conexão de Dados.

    ![Uma captura de tela mostrando a caixa de seleção que você precisa marcar para habilitar a Conexão de Dados para toda a sua organização.](images/data-connect-m365-enable-mgdc-for-org.png)

1. Insira **Aprovadores de** Solicitação de Consentimento (ou o  nome do grupo criado anteriormente) no grupo de usuários para tomar decisões de aprovação e selecione **Salvar**.

<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="58637-101">Antes de usar o Microsoft Graph dados Conexão pela primeira vez, você precisa configurar seu Microsoft 365 locatário.</span><span class="sxs-lookup"><span data-stu-id="58637-101">Prior to using Microsoft Graph Data Connect for the first time, you need to configure your Microsoft 365 tenant.</span></span> <span data-ttu-id="58637-102">Isso envolve a adição do serviço e a configuração de um grupo de segurança com permissões para aprovar solicitações de extração de dados.</span><span class="sxs-lookup"><span data-stu-id="58637-102">This involves turning on the service and configuring a security group with permissions to approve data extraction requests.</span></span>

## <a name="grant-azure-ad-users-the-global-administrator-role"></a><span data-ttu-id="58637-103">Conceder aos usuários do Azure AD a função de administrador global</span><span class="sxs-lookup"><span data-stu-id="58637-103">Grant Azure AD users the Global administrator role</span></span>

<span data-ttu-id="58637-104">Nesta etapa, você garantirá que dois usuários em seu Microsoft 365 locatário tenham a **função de** administrador global habilitada.</span><span class="sxs-lookup"><span data-stu-id="58637-104">In this step, you will ensure that two users in your Microsoft 365 tenant have the **Global administrator** role enabled.</span></span>

- <span data-ttu-id="58637-105">[Função de administrador global integrado](/azure/active-directory/roles/permissions-reference#global-administrator).</span><span class="sxs-lookup"><span data-stu-id="58637-105">[Global Administrator built-in role](/azure/active-directory/roles/permissions-reference#global-administrator).</span></span>
- <span data-ttu-id="58637-106">[Elevar o acesso para obter a função administrador global](/azure/role-based-access-control/elevate-access-global-admin).</span><span class="sxs-lookup"><span data-stu-id="58637-106">[Elevate access to gain the Global Administrator role](/azure/role-based-access-control/elevate-access-global-admin).</span></span>

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a><span data-ttu-id="58637-107">Configurar o grupo Graph aprovador de solicitação de consentimento Conexão Dados do Microsoft Conexão</span><span class="sxs-lookup"><span data-stu-id="58637-107">Configure Microsoft Graph Data Connect consent request approver group</span></span>

<span data-ttu-id="58637-108">Nesta etapa, você configurará seu locatário Microsoft 365 para habilitar o uso do Microsoft Graph Data Conexão.</span><span class="sxs-lookup"><span data-stu-id="58637-108">In this step, you will setup your Microsoft 365 tenant to enable usage of Microsoft Graph Data Connect.</span></span>

1. <span data-ttu-id="58637-109">Abra um navegador e vá para seu [Microsoft 365 Admin Portal](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="58637-109">Open a browser and go to your [Microsoft 365 Admin Portal](https://admin.microsoft.com/).</span></span>

1. <span data-ttu-id="58637-110">Na navegação da barra lateral, selecione **Grupos ativos**.</span><span class="sxs-lookup"><span data-stu-id="58637-110">On the sidebar navigation, select **Active Groups**.</span></span>
  
    ![Uma captura de tela mostrando os grupos ativos no Microsoft 365 de administração.](images/data-connect-m365-act-grp.png)

1. <span data-ttu-id="58637-112">Selecione o **botão Adicionar um grupo.**</span><span class="sxs-lookup"><span data-stu-id="58637-112">Select the **Add a group** button.</span></span>

1. <span data-ttu-id="58637-113">Use o seguinte para criar o novo grupo de segurança habilitado para **email** e selecione o **botão Adicionar.**</span><span class="sxs-lookup"><span data-stu-id="58637-113">Use the following to create the new **mail-enabled** security group and select the **Add** button.</span></span>
   - <span data-ttu-id="58637-114">**Tipo**: segurança habilitada para email</span><span class="sxs-lookup"><span data-stu-id="58637-114">**Type**: Mail-enabled security</span></span>

    ![Uma captura de tela mostrando um usuário selecionando a segurança habilitada para email para um novo grupo no Microsoft 365 de administração.](images/data-connect-m365-mail-sec.png)

   - <span data-ttu-id="58637-116">**Nome**: Aprovadores de Solicitação de Consentimento</span><span class="sxs-lookup"><span data-stu-id="58637-116">**Name**: Consent Request Approvers</span></span>

    ![Uma captura de tela mostrando um usuário está dando ao grupo um nome de "Aprovadores de Solicitação de Consentimento" no Microsoft 365 de administração.](images/data-connect-m365-cons-apprv.png)

   - <span data-ttu-id="58637-118">**Prefixo de Email**: consentrequestapprovers</span><span class="sxs-lookup"><span data-stu-id="58637-118">**Email Prefix**: consentrequestapprovers</span></span>

    ![Uma captura de tela mostrando um usuário criando o endereço de email para o grupo criado anteriormente no Microsoft 365 de administração.](images/data-connect-m365-cons-apprv-pref.png)

1. <span data-ttu-id="58637-120">**Pode levar até uma hora até** o grupo recém-criado aparecer na lista.</span><span class="sxs-lookup"><span data-stu-id="58637-120">**It can take up to an hour** before the newly created group shows up in the list.</span></span> <span data-ttu-id="58637-121">Quando o grupo tiver sido criado, selecione-o.</span><span class="sxs-lookup"><span data-stu-id="58637-121">When the group has been created, select it.</span></span>

1. <span data-ttu-id="58637-122">Vá para a **opção Grupos ativos** novamente e procure o grupo que você acabou de criar.</span><span class="sxs-lookup"><span data-stu-id="58637-122">Go to the **Active groups** option again and search for the group you just created.</span></span>

1. <span data-ttu-id="58637-123">Selecione o grupo e, na guia **Membros,** selecione **Exibir tudo e gerenciar membros**.</span><span class="sxs-lookup"><span data-stu-id="58637-123">Select the group and in the **Members** tab, select **View all and manage members**.</span></span>

1. <span data-ttu-id="58637-124">Adicione os dois usuários que você habilitaram a **função de** administrador global a esse novo grupo.</span><span class="sxs-lookup"><span data-stu-id="58637-124">Add the two users that you enabled the **Global administrator** role to this new group.</span></span>

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a><span data-ttu-id="58637-125">Habilitar o microsoft Graph dados Conexão seu locatário Microsoft 365 usuário</span><span class="sxs-lookup"><span data-stu-id="58637-125">Enable Microsoft Graph Data Connect in your Microsoft 365 tenant</span></span>

<span data-ttu-id="58637-126">Nesta etapa, você habilita o serviço microsoft Graph data Conexão no seu locatário Microsoft 365 usuário.</span><span class="sxs-lookup"><span data-stu-id="58637-126">In this step, you will enable the Microsoft Graph Data Connect service on your Microsoft 365 tenant.</span></span>

1. <span data-ttu-id="58637-127">Enquanto você ainda estiver Microsoft 365 Portal de Administração, selecione o item de menu configurações Configurações > **Org.**</span><span class="sxs-lookup"><span data-stu-id="58637-127">While you are still signed in to the Microsoft 365 Admin Portal, select the **Settings > Org settings** menu item.</span></span>

1. <span data-ttu-id="58637-128">Selecione o **serviço microsoft Graph dados Conexão** dados.</span><span class="sxs-lookup"><span data-stu-id="58637-128">Select the **Microsoft Graph Data Connect** service.</span></span>

    ![Uma captura de tela mostrando o "Serviços" na folha "Configurações da organização".](images/data-connect-m365-mgdc-toggle.png)

1. <span data-ttu-id="58637-131">Selecione a caixa de seleção que diz ativar ou desativar o **Microsoft Graph dados** Conexão toda a sua organização para habilitar dados Conexão.</span><span class="sxs-lookup"><span data-stu-id="58637-131">Select the checkbox that says **turn Microsoft Graph Data Connect on or off for your entire organization** to enable Data Connect.</span></span>

    ![Uma captura de tela mostrando a caixa de seleção que você precisa marcar para habilitar a Conexão dados para toda a sua organização.](images/data-connect-m365-enable-mgdc-for-org.png)

1. <span data-ttu-id="58637-133">Insira **Aprovadores de** Solicitação de Consentimento (ou o  nome do grupo criado anteriormente) no grupo de usuários para tomar decisões de aprovação e selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="58637-133">Enter **Consent Request Approvers** (or the name of the group you created previously) in the **group of users to make approval decisions** and select **Save**.</span></span>

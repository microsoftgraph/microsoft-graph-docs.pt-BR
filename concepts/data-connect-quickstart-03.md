<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="0ebfa-101">Neste exercício, você criará, executará e aprovará um pipeline da Fábrica de Dados do Azure para extrair dados do Microsoft 365 para um Blob do Azure Armazenamento para processamento adicional.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-101">In this exercise you will create, run, and approve an Azure Data Factory pipeline to extract data from Microsoft 365 to an Azure Storage Blob for additional processing.</span></span>

## <a name="create-a-microsoft-azure-active-directory-application-registration"></a><span data-ttu-id="0ebfa-102">Criar um registro Microsoft Azure Active Directory aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ebfa-102">Create a Microsoft Azure Active Directory application registration</span></span>

<span data-ttu-id="0ebfa-103">A primeira etapa é criar um aplicativo do Azure AD que será usado como entidade de segurança para executar o processo de extração de dados.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-103">The first step is to create an Azure AD application that will be used as the security principal to run the data extraction process.</span></span>

1. <span data-ttu-id="0ebfa-104">Abra um navegador e vá para o [Portal do Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="0ebfa-104">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="0ebfa-105">Entre usando uma conta com direitos **de administrador global** para seu Azure e Microsoft 365 locatários.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-105">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="0ebfa-106">Na navegação da barra lateral, selecione **Azure Active Directory** (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0ebfa-106">On the sidebar navigation, select **Azure Active Directory** (Azure AD).</span></span>

1. <span data-ttu-id="0ebfa-107">Na página Visão geral do Azure AD, selecione **Registros de** aplicativo na seção **Gerenciar** do menu.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-107">On the Azure AD Overview page, select **App registrations** from the **Manage** section of the menu.</span></span>

1. <span data-ttu-id="0ebfa-108">Selecione o **botão Novo registro.**</span><span class="sxs-lookup"><span data-stu-id="0ebfa-108">Select the **New registration** button.</span></span>

    ![Uma captura de tela mostrando os registros do aplicativo no serviço Azure Active Directory no portal do Azure.](images/data-connect-azure-aad-app-reg.png)

1. <span data-ttu-id="0ebfa-110">Use os seguintes valores para criar um novo aplicativo do Azure AD e selecione **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-110">Use the following values to create a new Azure AD application and select **Register**.</span></span>

   - <span data-ttu-id="0ebfa-111">**Nome**: Microsoft Graph Dados Conexão Transferência de Dados</span><span class="sxs-lookup"><span data-stu-id="0ebfa-111">**Name**: Microsoft Graph Data Connect Data Transfer</span></span>
   - <span data-ttu-id="0ebfa-112">**Tipos de conta com suporte**: Somente contas neste diretório organizacional.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-112">**Supported account types**: Accounts in this organizational directory only.</span></span>
   - <span data-ttu-id="0ebfa-113">**URI de redirecionamento**: deixe os valores padrão.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-113">**Redirect URI**: Leave the default values.</span></span>

    ![Uma captura de tela mostrando as etapas para registrar um novo registro de aplicativo no portal do Azure.](images/data-connect-aad-redirect-uri.png)

1. <span data-ttu-id="0ebfa-115">Localize **a ID do Aplicativo (cliente)** e copie-a como você precisará mais adiante neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-115">Locate the **Application (client) ID** and copy it as you will need it later in this tutorial.</span></span> <span data-ttu-id="0ebfa-116">Isso será chamado de ID da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-116">This will be referred to as the service principal ID.</span></span>

1. <span data-ttu-id="0ebfa-117">Localize **a ID de Diretório (locatário)** e copie-a como você precisará mais adiante neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-117">Locate the **Directory (tenant) ID** and copy it as you will need it later in this tutorial.</span></span> <span data-ttu-id="0ebfa-118">Isso será chamado de ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-118">This will be referred to as the tenant ID.</span></span>

1. <span data-ttu-id="0ebfa-119">Na navegação na barra lateral, selecione **Certificados e segredos em** **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-119">On the sidebar navigation, select **Certificates and secrets** under **Manage**.</span></span>

1. <span data-ttu-id="0ebfa-120">Selecione o **botão Novo segredo do cliente.**</span><span class="sxs-lookup"><span data-stu-id="0ebfa-120">Select the **New client secret button**.</span></span> <span data-ttu-id="0ebfa-121">Definir *Descrição* como qualquer nome, definir **Expira como** qualquer valor no menu suspenso e escolha **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-121">Set *Description* to any name, set **Expires** to any value in the dropdown and choose **Add**.</span></span>

    ![Uma captura de tela mostrando o processo para criar um novo segredo do cliente no portal do Azure.](images/data-connect-aad-certs-secrets.png)

    - <span data-ttu-id="0ebfa-123">Depois que o segredo do cliente for criado, salve o **Valor** em algum lugar seguro, pois ele não estará mais disponível posteriormente e você precisará criar um novo.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-123">After the client secret is created, make sure you save the **Value** somewhere safe, as it will no longer be available later, and you will need to create a new one.</span></span>
    - <span data-ttu-id="0ebfa-124">Isso será referenciado como a chave principal do serviço.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-124">This will be referenced as the service principal key.</span></span>

1. <span data-ttu-id="0ebfa-125">Na navegação da barra lateral do aplicativo, selecione **Proprietários**.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-125">On the sidebar navigation for the application, select **Owners**.</span></span>

1. <span data-ttu-id="0ebfa-126">Verifique se sua conta está listada como proprietária do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-126">Verify that your account is listed as an owner for the application.</span></span> <span data-ttu-id="0ebfa-127">Se ele não estiver listado como proprietário, adicione-o.</span><span class="sxs-lookup"><span data-stu-id="0ebfa-127">If it isn't listed as an owner, add it.</span></span>

    ![Uma captura de tela mostrando um usuário verificando se sua conta está definida como proprietária para o registro do aplicativo no portal do Azure.](images/data-connect-aad-app-owners.png)

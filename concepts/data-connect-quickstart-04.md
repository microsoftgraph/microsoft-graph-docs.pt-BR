<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="fa87a-101">Nesta etapa, você criará uma conta do Azure Armazenamento onde conexão de dados do Microsoft Graph armazenará os dados extraídos do Microsoft 365 para processamento posterior.</span><span class="sxs-lookup"><span data-stu-id="fa87a-101">In this step you will create an Azure Storage account where Microsoft Graph data connect will store the data extracted from Microsoft 365 for further processing.</span></span>

1. <span data-ttu-id="fa87a-102">Abra um navegador e vá para o [Portal do Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="fa87a-102">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="fa87a-103">Entre usando uma conta com direitos **de administrador global** para seu Azure e Microsoft 365 locatários.</span><span class="sxs-lookup"><span data-stu-id="fa87a-103">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="fa87a-104">Na navegação da barra lateral, selecione **Criar um recurso**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-104">On the sidebar navigation, select **Create a resource**.</span></span>

1. <span data-ttu-id="fa87a-105">Encontre o **Armazenamento tipo** de recurso Conta e use os seguintes valores para cria-lo e selecione Revisar **+ criar**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-105">Find the **Storage Account** resource type and use the following values to create it, then select **Review + create**.</span></span>

    - <span data-ttu-id="fa87a-106">**Assinatura**: selecione sua assinatura do Azure</span><span class="sxs-lookup"><span data-stu-id="fa87a-106">**Subscription**: select your Azure subscription</span></span>
    - <span data-ttu-id="fa87a-107">**Grupo de recursos**: GraphDataConnect (ou selecione um grupo de recursos existente)</span><span class="sxs-lookup"><span data-stu-id="fa87a-107">**Resource group**: GraphDataConnect (or select an existing resource group)</span></span>
    - <span data-ttu-id="fa87a-108">**Armazenamento da conta**: mgdcm365datastore</span><span class="sxs-lookup"><span data-stu-id="fa87a-108">**Storage account name**: mgdcm365datastore</span></span>
    - <span data-ttu-id="fa87a-109">**Região**: escolha uma região do Azure na mesma região que sua Microsoft 365 região</span><span class="sxs-lookup"><span data-stu-id="fa87a-109">**Region**: pick an Azure region in the same region as your Microsoft 365 region</span></span>
    - <span data-ttu-id="fa87a-110">**Desempenho**: Standard</span><span class="sxs-lookup"><span data-stu-id="fa87a-110">**Performance**: Standard</span></span>
    - <span data-ttu-id="fa87a-111">**Redundância**: Armazenamento geo-redundante (GRS)</span><span class="sxs-lookup"><span data-stu-id="fa87a-111">**Redundancy**: Geo-redundant storage (GRS)</span></span>
    - <span data-ttu-id="fa87a-112">**Guia Avançado**:</span><span class="sxs-lookup"><span data-stu-id="fa87a-112">**Advanced tab**:</span></span>
      - <span data-ttu-id="fa87a-113">**Camada de acesso**: Hot</span><span class="sxs-lookup"><span data-stu-id="fa87a-113">**Access tier**: Hot</span></span>

1. <span data-ttu-id="fa87a-114">Revise se as configurações corresponderão às mostradas na etapa anterior e selecione **Criar**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-114">Review that the settings match those shown in the previous step and select **Create**.</span></span>

1. <span data-ttu-id="fa87a-115">Depois que a conta Armazenamento do Azure tiver sido criada, conceda ao aplicativo do Azure AD criado anteriormente o acesso adequado a ela.</span><span class="sxs-lookup"><span data-stu-id="fa87a-115">After the Azure Storage account has been created, grant the Azure AD application previously created the proper access to it.</span></span>

    1. <span data-ttu-id="fa87a-116">Selecione a **conta do Azure Armazenamento**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-116">Select the **Azure Storage account**.</span></span>
    2. <span data-ttu-id="fa87a-117">No menu barra lateral, selecione **Controle de acesso (IAM)**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-117">On the sidebar menu, select **Access control (IAM)**.</span></span>
    3. <span data-ttu-id="fa87a-118">Selecione o **botão Adicionar** no bloco Adicionar **uma atribuição de** função.</span><span class="sxs-lookup"><span data-stu-id="fa87a-118">Select the **Add** button in the **Add a role assignment** block.</span></span>
    4. <span data-ttu-id="fa87a-119">Use os seguintes valores para encontrar o aplicativo selecionado anteriormente para conceder Armazenamento função de Colaborador de Dados de **Blob** e, em seguida, **selecione Salvar**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-119">Use the following values to find the application you previously selected to grant it the **Storage Blob Data Contributor** role, then select **Save**.</span></span>

        - <span data-ttu-id="fa87a-120">**Função**: Armazenamento blob data contributor</span><span class="sxs-lookup"><span data-stu-id="fa87a-120">**Role**: Storage Blob Data Contributor</span></span>
        - <span data-ttu-id="fa87a-121">**Atribuir acesso a**: Usuário, grupo ou entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="fa87a-121">**Assign access to**: User, group or service principal</span></span>
        - <span data-ttu-id="fa87a-122">**Selecione**: conexão de dados do Microsoft Graph transferência de dados (o nome do aplicativo do Azure AD criado anteriormente)</span><span class="sxs-lookup"><span data-stu-id="fa87a-122">**Select**: Microsoft Graph data connect Data Transfer (the name of the Azure AD application you created previously)</span></span>

        ![Uma captura de tela mostrando a atribuição de função adequada para o aplicativo do Microsoft Graph Data Conexão na conta do Azure Armazenamento no portal do Azure.](images/data-connect-azure-storage-role.png)

1. <span data-ttu-id="fa87a-124">Crie um novo contêiner na **conta mgdcm365datastore** Azure Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="fa87a-124">Create a new container in the **mgdcm365datastore** Azure Storage account.</span></span>

    1. <span data-ttu-id="fa87a-125">Selecione a **conta mgdcm365datastore** do Azure Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="fa87a-125">Select the **mgdcm365datastore** Azure Storage account.</span></span>
    2. <span data-ttu-id="fa87a-126">No menu barra lateral, selecione **Contêineres** na seção Serviço **blob.**</span><span class="sxs-lookup"><span data-stu-id="fa87a-126">On the sidebar menu, select **Containers** under the **Blob** service section.</span></span>
    3. <span data-ttu-id="fa87a-127">Selecione o **botão +Contêiner** na parte superior da página e use os seguintes valores e selecione **Criar**.</span><span class="sxs-lookup"><span data-stu-id="fa87a-127">Select the **+Container** button at the top of the page and use the following values and then select **Create**.</span></span>

        - <span data-ttu-id="fa87a-128">**Nome**: m365mails</span><span class="sxs-lookup"><span data-stu-id="fa87a-128">**Name**: m365mails</span></span>
        - <span data-ttu-id="fa87a-129">**Nível de acesso público**: Privado (sem acesso anônimo)</span><span class="sxs-lookup"><span data-stu-id="fa87a-129">**Public access level**: Private (no anonymous access)</span></span>

        ![Uma captura de tela mostrando a criação de um novo contêiner chamado m365mails nos contêineres de blob Armazenamento conta no portal do Azure.](images/data-connect-azure-storage-container.png)

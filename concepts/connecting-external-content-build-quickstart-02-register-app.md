<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="3c1f7-101">Depois de todos os pré-requisitos, você poderá registrar um aplicativo no centro de administração do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-101">After all the prerequisites are in place, you will be able to register an application in the Azure AD admin center.</span></span> <span data-ttu-id="3c1f7-102">O registro é necessário para autenticar o aplicativo e usá-lo para fazer chamadas para a API de conectores Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-102">The registration is necessary in order to authenticate the application and use it to make calls to the Microsoft Graph connectors API.</span></span>

1. <span data-ttu-id="3c1f7-103">Vá para o Azure Active Directory [de administração e](https://aad.portal.azure.com/) entre com uma conta de administrador.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-103">Go to the [Azure Active Directory admin center](https://aad.portal.azure.com/) and sign in with an administrator account.</span></span>
2. <span data-ttu-id="3c1f7-104">No painel esquerdo, selecione **Azure Active Directory**, e em **Gerenciar**, selecione Registros **de aplicativo.**</span><span class="sxs-lookup"><span data-stu-id="3c1f7-104">On the left pane, select **Azure Active Directory**, and under **Manage**, select **App registrations**.</span></span>
3. <span data-ttu-id="3c1f7-105">Selecione **Novo registro**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-105">Select **New registration**.</span></span>

    ![Captura de tela mostrando a seção "registros de aplicativo"](images/connectors-images/build2.png)

4. <span data-ttu-id="3c1f7-107">Conclua **o formulário Registrar um** aplicativo com os seguintes valores e selecione **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-107">Complete the **Register an application** form with the following values, then select **Register**.</span></span>

    <span data-ttu-id="3c1f7-108">a.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-108">a.</span></span> <span data-ttu-id="3c1f7-109">**Nome**: Conector de Inventário de Partes</span><span class="sxs-lookup"><span data-stu-id="3c1f7-109">**Name**: Parts Inventory Connector</span></span>

    <span data-ttu-id="3c1f7-110">b.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-110">b.</span></span> <span data-ttu-id="3c1f7-111">**Tipos de conta com suporte:** Contas somente neste diretório organizacional (somente microsoft - locatário único)</span><span class="sxs-lookup"><span data-stu-id="3c1f7-111">**Supported account types**: Accounts in this organizational directory only (Microsoft only - Single tenant)</span></span>

    <span data-ttu-id="3c1f7-112">c.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-112">c.</span></span> <span data-ttu-id="3c1f7-113">**URI de redirecionamento**: deixar em branco</span><span class="sxs-lookup"><span data-stu-id="3c1f7-113">**Redirect URI**: Leave blank</span></span>

    ![Captura de tela mostrando a seção "registrar um aplicativo"](images/connectors-images/build3-contoso-register-app.png)

5. <span data-ttu-id="3c1f7-115">Na página Visão geral do Conector de Inventário de Partes, copie os valores de ID de Aplicativo (cliente) e ID de Diretório **(locatário).**</span><span class="sxs-lookup"><span data-stu-id="3c1f7-115">On the Parts Inventory Connector overview page, copy the values of **Application (client) ID and Directory (tenant) ID**.</span></span> <span data-ttu-id="3c1f7-116">Você precisará dos dois na seção a seguir.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-116">You will need both in the following section.</span></span>

    ![Captura de tela mostrando a seção "conector de inventário de partes"](images/connectors-images/build3-contoso-partsinv.png)

6. <span data-ttu-id="3c1f7-118">Selecione **Permissões de API em** **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-118">Select **API Permissions** under **Manage**.</span></span>
7. <span data-ttu-id="3c1f7-119">Selecione **Adicionar uma permissão** e selecione Microsoft **Graph**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-119">Select **Add a permission**, then select **Microsoft Graph**.</span></span>
8. <span data-ttu-id="3c1f7-120">Selecione **Permissões de aplicativo** e selecione a permissão **ExternalItem.ReadWrite.All.**</span><span class="sxs-lookup"><span data-stu-id="3c1f7-120">Select **Application permissions**, then select the **ExternalItem.ReadWrite.All** permission.</span></span> <span data-ttu-id="3c1f7-121">Selecione **Adicionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-121">Select **Add permissions**.</span></span>

    ![Captura de tela mostrando a seção "solicitar permissões de API"](images/connectors-images/build4.png)

9. <span data-ttu-id="3c1f7-123">Selecione **Conceder consentimento de administrador para {TENANT}e** selecione **Sim** quando solicitado.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-123">Select **Grant admin consent for {TENANT},** then select **Yes** when prompted.</span></span>

    ![Captura de tela mostrando a seção "permissões de api do conector de inventário de partes"](images/connectors-images/build5.png)

10. <span data-ttu-id="3c1f7-125">Selecione **Certificados &amp; segredos em** **Gerenciar** , em seguida, selecione Novo segredo **do cliente**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-125">Select **Certificates &amp; secrets** under **Manage** , then select **New client secret**.</span></span>
11. <span data-ttu-id="3c1f7-126">Insira uma descrição e escolha um tempo de expiração para o segredo e selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-126">Enter a description and choose an expiration time for the secret, then select **Add**.</span></span>

    ![Captura de tela mostrando a seção "certificados e segredos do conector de inventário de partes"](images/connectors-images/build6.png)

12. <span data-ttu-id="3c1f7-128">Copie e salve o novo segredo, você precisará dele na seção a seguir.</span><span class="sxs-lookup"><span data-stu-id="3c1f7-128">Copy and save the new secret, you will need it in the following section.</span></span>

<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="1864b-101">Um Microsoft 365 administrador tem a capacidade de aprovar ou negar solicitações de consentimento.</span><span class="sxs-lookup"><span data-stu-id="1864b-101">A Microsoft 365 administrator has the ability to approve or deny consent requests.</span></span> <span data-ttu-id="1864b-102">Isso pode ser feito por meio do Microsoft 365 Admin Center ou programaticamente por meio do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1864b-102">This can be done via the Microsoft 365 Admin Center or programmatically via PowerShell.</span></span>

## <a name="approve-consent-requests"></a><span data-ttu-id="1864b-103">Aprovar solicitações de consentimento</span><span class="sxs-lookup"><span data-stu-id="1864b-103">Approve consent requests</span></span>

# <a name="microsoft-365-admin-center"></a>[<span data-ttu-id="1864b-104">Microsoft 365 Centro de administração</span><span class="sxs-lookup"><span data-stu-id="1864b-104">Microsoft 365 Admin Center</span></span>](#tab/Microsoft365)

1. <span data-ttu-id="1864b-105">Abra um navegador e vá para seu [Microsoft 365 Admin Portal](https://admin.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="1864b-105">Open a browser and go to your [Microsoft 365 Admin Portal](https://admin.microsoft.com).</span></span>

1. <span data-ttu-id="1864b-106">Para aprovar ou negar solicitações de consentimento, acesse [Acesso Privilegiado.](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess)</span><span class="sxs-lookup"><span data-stu-id="1864b-106">To approve or deny consent requests, go to [Privileged Access](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess).</span></span>

1. <span data-ttu-id="1864b-107">Selecione uma Solicitação pendente **de Acesso a Dados**.</span><span class="sxs-lookup"><span data-stu-id="1864b-107">Select a pending **Data Access Request**.</span></span>

1. <span data-ttu-id="1864b-108">Na chamada **Solicitação de Acesso** a Dados, selecione o **botão Aprovar.**</span><span class="sxs-lookup"><span data-stu-id="1864b-108">In the **Data Access Request** call out, select the **Approve** button.</span></span>

    ![Uma captura de tela mostrando uma solicitação de acesso a dados aguardando aprovação de consentimento no Microsoft 365 de administração.](images/data-connect-m365-approve.png)

# <a name="powershell"></a>[<span data-ttu-id="1864b-110">PowerShell</span><span class="sxs-lookup"><span data-stu-id="1864b-110">PowerShell</span></span>](#tab/PowerShell)

1. <span data-ttu-id="1864b-111">Abra o PowerShell do Windows.</span><span class="sxs-lookup"><span data-stu-id="1864b-111">Open Windows PowerShell.</span></span>
1. <span data-ttu-id="1864b-112">Certifique-se de que sua sessão do PowerShell tenha habilitado scripts assinados remotamente.</span><span class="sxs-lookup"><span data-stu-id="1864b-112">Ensure that your PowerShell session has enabled remotely signed scripts.</span></span>

    ```powershell
    Set-ExecutionPolicy RemoteSigned
    ```

1. <span data-ttu-id="1864b-113">Conexão para Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1864b-113">Connect to Exchange Online.</span></span>

    1. <span data-ttu-id="1864b-114">Obtenha uma credencial de logom executando o PowerShell a seguir.</span><span class="sxs-lookup"><span data-stu-id="1864b-114">Obtain a sign in credential by executing the following PowerShell.</span></span> <span data-ttu-id="1864b-115">Entre usando um usuário diferente do que aquele que criou e iniciou o pipeline da Fábrica de Dados do Azure, que tem a função de administrador **global** aplicada, que é membro do grupo que tem direitos para aprovar solicitações para dados no Microsoft 365 e tem a autenticação multifafação habilitada.</span><span class="sxs-lookup"><span data-stu-id="1864b-115">Sign in using a different user than one that created and started the Azure Data Factory pipeline, who has the **Global administrator** role applied, who is a member of the group that has rights to approve requests to data in Microsoft 365, and has multi-factor authentication enabled.</span></span>

        ```powershell
        $UserCredential = Get-Credential
        ```

    1. <span data-ttu-id="1864b-116">Crie uma nova sessão Exchange Online do PowerShell e carregue -a (importe).</span><span class="sxs-lookup"><span data-stu-id="1864b-116">Create a new Exchange Online PowerShell session and load (import) it.</span></span>

        ```powershell
        $Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://ps.protection.outlook.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection
        Import-PSSession $Session -DisableNameChecking
        ```

        > [!IMPORTANT]
        > <span data-ttu-id="1864b-117">Depois de terminar essa sessão, certifique-se de desconectar da sessão usando o comando do PowerShell `Remove-PSSession $Session` .</span><span class="sxs-lookup"><span data-stu-id="1864b-117">After you are finished with this session, be sure you you disconnect from the session using the PowerShell command `Remove-PSSession $Session`.</span></span> <span data-ttu-id="1864b-118">Exchange Online permite apenas três sessões do PowerShell remotas abertas para proteger contra ataques de negação de serviço (DoS).</span><span class="sxs-lookup"><span data-stu-id="1864b-118">Exchange Online only allows for three open remote PowerShell sessions to protect against denial-of-service (DoS) attacks.</span></span> <span data-ttu-id="1864b-119">Se você simplesmente fechar a janela do PowerShell, ela deixará a conexão aberta.</span><span class="sxs-lookup"><span data-stu-id="1864b-119">If you simply close the PowerShell window, it will leave the connection open.</span></span>

1. <span data-ttu-id="1864b-120">Obter uma lista de todas as solicitações de dados pendentes conexão de dados do Microsoft Graph executando o PowerShell a seguir.</span><span class="sxs-lookup"><span data-stu-id="1864b-120">Get a list of all pending data requests from Microsoft Graph data connect by executing the following PowerShell.</span></span>

    ```powershell
    Get-ElevatedAccessRequest | where {$_.RequestStatus -eq 'Pending'} | select RequestorUPN, Service, Identity, RequestedAccess | fl
    ```

    - <span data-ttu-id="1864b-121">Examine a lista de solicitações de acesso a dados retornadas.</span><span class="sxs-lookup"><span data-stu-id="1864b-121">Examine the list of data access requests returned.</span></span> <span data-ttu-id="1864b-122">Na imagem a seguir, observe que há duas solicitações pendentes.</span><span class="sxs-lookup"><span data-stu-id="1864b-122">In the following image, notice there are two pending requests.</span></span>

        ![Uma captura de tela mostrando uma lista de solicitações pendentes formatadas como uma lista em um console do PowerShell.](images/data-connect-ps-pending-requests.png)

1. <span data-ttu-id="1864b-124">Aprove um acesso de dados retornado na etapa anterior copiando o GUID de identidade de uma solicitação executando o PowerShell a seguir.</span><span class="sxs-lookup"><span data-stu-id="1864b-124">Approve a data access returned in the previous step by copying the Identity GUID of a request by executing the following PowerShell.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1864b-125">Substitua o GUID no trecho de código a seguir pelo GUID dos resultados da etapa anterior.</span><span class="sxs-lookup"><span data-stu-id="1864b-125">Replace the GUID in the following code snippet with the GUID from the results of the previous step.</span></span>

    ```powershell
    Approve-ElevatedAccessRequest -RequestId fa041379-0000-0000-0000-7cd5691484bd -Comment 'approval request granted'
    ```

1. <span data-ttu-id="1864b-126">Depois de alguns instantes, você deve ver a página de status da atualização de executar atividade para mostrar que agora está _extraindo dados_.</span><span class="sxs-lookup"><span data-stu-id="1864b-126">After a few moments, you should see the status page for the activity run update to show it is now _extracting data_.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço Fábrica de Dados onde o status da carga agora está sendo mostrado como "Extração de dados".](images/data-connect-adf-extraction-approved.png)

1. <span data-ttu-id="1864b-128">Esse processo de extração de dados pode levar algum tempo, dependendo do tamanho do seu locatário Microsoft 365 local.</span><span class="sxs-lookup"><span data-stu-id="1864b-128">This process of extracting the data can take some time depending on the size of your Microsoft 365 tenant.</span></span>

---

## <a name="verify-extracted-data-from-microsoft-365-to-azure-storage-blob"></a><span data-ttu-id="1864b-129">Verificar dados extraídos do Microsoft 365 para o Azure Armazenamento Blob</span><span class="sxs-lookup"><span data-stu-id="1864b-129">Verify extracted data from Microsoft 365 to Azure Storage Blob</span></span>

1. <span data-ttu-id="1864b-130">Abra um navegador e vá para o [Portal do Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="1864b-130">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="1864b-131">Entre usando uma conta com direitos **de administrador global** para seu Azure e Microsoft 365 locatários.</span><span class="sxs-lookup"><span data-stu-id="1864b-131">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="1864b-132">Na navegação da barra lateral, selecione o item de menu **Todos os recursos.**</span><span class="sxs-lookup"><span data-stu-id="1864b-132">On the sidebar navigation, select the **All resources** menu item.</span></span>

1. <span data-ttu-id="1864b-133">Na lista de recursos, selecione a conta de Armazenamento **do Azure** que você criou anteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="1864b-133">In the list of resources, select the **Azure Storage account** you created previously in this tutorial.</span></span>

1. <span data-ttu-id="1864b-134">No menu de navegação da barra lateral, selecione **Blobs** na folha de Armazenamento **conta do Azure.**</span><span class="sxs-lookup"><span data-stu-id="1864b-134">On the sidebar navigation menu, select **Blobs** from the **Azure Storage account** blade.</span></span>

1. <span data-ttu-id="1864b-135">Selecione o **contêiner** criado anteriormente neste tutorial que você configurou o pipeline da Fábrica de Dados do Azure como o pia para os dados extraídos.</span><span class="sxs-lookup"><span data-stu-id="1864b-135">Select the **container** created previously in this tutorial that you configured the Azure Data Factory pipeline as the sink for the extracted data.</span></span> <span data-ttu-id="1864b-136">Você deve ver dados neste contêiner agora.</span><span class="sxs-lookup"><span data-stu-id="1864b-136">You should see data in this container now.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço Armazenamento conta.](images/data-connect-adf-extracted-data-in-blob.png)

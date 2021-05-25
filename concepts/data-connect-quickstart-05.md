<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="00034-101">A próxima etapa é usar a Fábrica de Dados do Azure para criar um pipeline para extrair os dados do Microsoft 365 para a conta Armazenamento do Azure usando conexão de dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="00034-101">The next step is to use the Azure Data Factory to create a pipeline to extract the data from Microsoft 365 to the Azure Storage account using Microsoft Graph data connect.</span></span>

## <a name="create-an-azure-data-factory-pipeline"></a><span data-ttu-id="00034-102">Criar um pipeline do Azure Data Factory</span><span class="sxs-lookup"><span data-stu-id="00034-102">Create an Azure Data Factory pipeline</span></span>

1. <span data-ttu-id="00034-103">Abra um navegador e vá para o [Portal do Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="00034-103">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="00034-104">Entre usando uma conta com direitos **de administrador global** para seu Azure e Microsoft 365 locatários.</span><span class="sxs-lookup"><span data-stu-id="00034-104">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="00034-105">Na navegação da barra lateral, selecione **Criar um recurso**.</span><span class="sxs-lookup"><span data-stu-id="00034-105">On the sidebar navigation, select **Create a resource**.</span></span>

1. <span data-ttu-id="00034-106">Encontre o **tipo de recurso Fábrica** de Dados e use os seguintes valores para cria-lo e selecione **Criar**.</span><span class="sxs-lookup"><span data-stu-id="00034-106">Find the **Data Factory** resource type and use the following values to create it, then select **Create**.</span></span>

    1. <span data-ttu-id="00034-107">**Assinatura**: selecione sua assinatura do Azure</span><span class="sxs-lookup"><span data-stu-id="00034-107">**Subscription**: select your Azure subscription</span></span>
    2. <span data-ttu-id="00034-108">**Grupo de recursos**: GraphDataConnect</span><span class="sxs-lookup"><span data-stu-id="00034-108">**Resource group**: GraphDataConnect</span></span>
    3. <span data-ttu-id="00034-109">**Região**: escolha uma região do Azure na mesma região que sua Microsoft 365 região</span><span class="sxs-lookup"><span data-stu-id="00034-109">**Region**: pick an Azure region in the same region as your Microsoft 365 region</span></span>
    4. <span data-ttu-id="00034-110">**Nome**: dfM365toBlobStorage</span><span class="sxs-lookup"><span data-stu-id="00034-110">**Name**: dfM365toBlobStorage</span></span>
    5. <span data-ttu-id="00034-111">**Versão**: V2</span><span class="sxs-lookup"><span data-stu-id="00034-111">**Version**: V2</span></span>

        ![Uma captura de tela mostrando a criação bem-sucedida do novo serviço da Fábrica de Dados do Azure no portal do Azure.](images/data-connect-adf-create.png)

    6. <span data-ttu-id="00034-113">Na guia **Configuração do Git,** configure o Git ou selecione a opção _Configurar o Git posteriormente._</span><span class="sxs-lookup"><span data-stu-id="00034-113">In the **Git configuration** tab, make sure you either configure Git or select the option _Configure Git later_.</span></span>

1. <span data-ttu-id="00034-114">Depois que o recurso da Fábrica de Dados do Azure for criado, selecione o bloqueio Autor e **Monitor** para iniciar o editor de tela inteira do Azure Data Factory.</span><span class="sxs-lookup"><span data-stu-id="00034-114">After the Azure Data Factory resource is created, select the **Author and Monitor** tile to launch the Azure Data Factory full screen editor.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do Portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-auth-and-mon.png)

1. <span data-ttu-id="00034-117">Alternar da **visão geral** para a **experiência Gerenciar** selecionando-a na navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="00034-117">Switch from the **Overview** to the **Manage** experience by selecting it from the left-hand navigation.</span></span>

1. <span data-ttu-id="00034-118">Por padrão, a Fábrica de Dados do Azure usará um tempo de execução de integração que está resolvendo automaticamente a região.</span><span class="sxs-lookup"><span data-stu-id="00034-118">By default, the Azure Data Factory will use an integration runtime that is auto-resolving the region.</span></span> <span data-ttu-id="00034-119">Como o data Conexão requer que sua origem, destino e tempo de execução de integração existam na mesma região Microsoft 365, recomendamos que você crie um novo tempo de execução de integração com uma região fixa.</span><span class="sxs-lookup"><span data-stu-id="00034-119">Because Data Connect requires that your source and destination, and integration runtime to exist in the same Microsoft 365 region, we recommend that you create a new integration runtime with a fixed region.</span></span>

    1. <span data-ttu-id="00034-120">Selecione **Tempos de execução de**  >  **integração Novo**.</span><span class="sxs-lookup"><span data-stu-id="00034-120">Select **Integration runtimes** > **New**.</span></span>
    2. <span data-ttu-id="00034-121">Selecione **Azure, Auto-hospedado e** selecione **Continuar**.</span><span class="sxs-lookup"><span data-stu-id="00034-121">Select **Azure, Self-Hosted** and select **Continue**.</span></span>
    3. <span data-ttu-id="00034-122">Selecione **Azure** para ambiente de rede e selecione **Continuar**.</span><span class="sxs-lookup"><span data-stu-id="00034-122">Select **Azure** for network environment and select **Continue**.</span></span>

        ![Uma captura de tela mostrando a interface do usuário do Portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-network.png)

    4. <span data-ttu-id="00034-125">Use os detalhes a seguir para concluir o formulário na tela final e selecione **Criar**.</span><span class="sxs-lookup"><span data-stu-id="00034-125">Use the following details to complete the form on the final screen and then select **Create**.</span></span>

        - <span data-ttu-id="00034-126">**Nome**: nome do tempo de execução de integração</span><span class="sxs-lookup"><span data-stu-id="00034-126">**Name**: name of your integration runtime</span></span>
        - <span data-ttu-id="00034-127">**Descrição**: insira uma descrição</span><span class="sxs-lookup"><span data-stu-id="00034-127">**Description**: enter a description</span></span>
        - <span data-ttu-id="00034-128">**Região**: selecione a região que corresponde ao seu Microsoft 365 região</span><span class="sxs-lookup"><span data-stu-id="00034-128">**Region**: select the region that matches your Microsoft 365 region</span></span>
        - <span data-ttu-id="00034-129">**Configuração de rede virtual (visualização)**: Desabilitada</span><span class="sxs-lookup"><span data-stu-id="00034-129">**Virtual network configuration (preview)**: Disabled</span></span>

1. <span data-ttu-id="00034-130">Alternar da **experiência Gerenciar** para **o Autor** selecionando-a na navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="00034-130">Switch from the **Manage** to the **Author** experience by selecting it from the left-hand navigation.</span></span>
1. <span data-ttu-id="00034-131">Crie um novo pipeline selecionando o **ícone de a** mais e, em seguida, **pipeline**.</span><span class="sxs-lookup"><span data-stu-id="00034-131">Create a new pipeline by selecting the **plus** icon, then **pipeline**.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-pipeline-create.png)

    - <span data-ttu-id="00034-134">Arraste a **atividade Copiar Dados** da seção Mover e **Transformar** para a superfície de design.</span><span class="sxs-lookup"><span data-stu-id="00034-134">Drag the **Copy Data** activity from the **Move and Transform** section onto the design surface.</span></span>

        ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-pipeline-copy-data.png)

    - <span data-ttu-id="00034-137">Selecione a atividade no designer.</span><span class="sxs-lookup"><span data-stu-id="00034-137">Select the activity in the designer.</span></span>
    - <span data-ttu-id="00034-138">Selecione a **guia Geral** e dê a ela um nome e uma descrição.</span><span class="sxs-lookup"><span data-stu-id="00034-138">Select the **General** tab and give it a name and description.</span></span>

      - <span data-ttu-id="00034-139">**Nome**: CopyFromM365toBlobStorage</span><span class="sxs-lookup"><span data-stu-id="00034-139">**Name**: CopyFromM365toBlobStorage</span></span>
      - <span data-ttu-id="00034-140">**Descrição**: Uma descrição que você deseja.</span><span class="sxs-lookup"><span data-stu-id="00034-140">**Description**: A description you want.</span></span>

    - <span data-ttu-id="00034-141">No painel editor de atividades abaixo do designer, selecione a guia **Origem** e selecione **Novo**.</span><span class="sxs-lookup"><span data-stu-id="00034-141">In the activity editor pane below the designer, select the **Source** tab, then select **New**.</span></span>
    - <span data-ttu-id="00034-142">Localize o **Office 365** de dados, selecione-o e selecione o **botão Continuar.**</span><span class="sxs-lookup"><span data-stu-id="00034-142">Locate the dataset **Office 365**, select it and then select the **Continue** button.</span></span>

        ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-pipeline-dataset.png)

    - <span data-ttu-id="00034-145">O designer atualizará a guia **Fonte** com as configurações Microsoft 365 conector.</span><span class="sxs-lookup"><span data-stu-id="00034-145">The designer will update the **Source** tab with the Microsoft 365 connector settings.</span></span>
    - <span data-ttu-id="00034-146">Selecione a **opção Abrir** ao lado do campo **Conjuntos de** dados de origem.</span><span class="sxs-lookup"><span data-stu-id="00034-146">Select the **Open** option next to the **Source dataset** field.</span></span>
    - <span data-ttu-id="00034-147">Nas configurações da tabela, selecione a guia **Conexão** e, em seguida, o **botão Novo.**</span><span class="sxs-lookup"><span data-stu-id="00034-147">In the table settings, select the **Connection** tab, then the **New** button.</span></span>
    - <span data-ttu-id="00034-148">Na caixa de diálogo exibida, insira a ID de Aplicativo e a   **ID** secreta do aplicativo Azure AD criadas anteriormente nos campos de chave principal do serviço e da chave principal do serviço, respectivamente, e selecione **Criar**. </span><span class="sxs-lookup"><span data-stu-id="00034-148">In the dialog that appears, enter the previously created Azure AD application's **Application ID** and **Secret ID** in the **Service principal ID** and **Service principal key** fields respectively, then select **Create**.</span></span>
    - <span data-ttu-id="00034-149">Selecione o tempo de execução de integração criado anteriormente no Conexão por meio do menu suspenso **tempo de execução de** integração.</span><span class="sxs-lookup"><span data-stu-id="00034-149">Select the integration runtime you previously created in the **Connect via integration runtime** dropdown.</span></span>

        ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-linked-service.png)

    - <span data-ttu-id="00034-152">Após criar a Microsoft 365, para o campo **Tabela,** selecione **BasicDataSet_v0. Message_v0**.</span><span class="sxs-lookup"><span data-stu-id="00034-152">After creating the Microsoft 365 connection, for the **Table** field, select **BasicDataSet_v0.Message_v0**.</span></span>
    - <span data-ttu-id="00034-153">Alternar do **Office365Table para o** **Pipeline > Source**.</span><span class="sxs-lookup"><span data-stu-id="00034-153">Switch from **Office365Table** to **Pipeline > Source**.</span></span> <span data-ttu-id="00034-154">Use os seguintes valores para o **filtro Date.**</span><span class="sxs-lookup"><span data-stu-id="00034-154">Use the following values for the **Date filter**.</span></span>

      - <span data-ttu-id="00034-155">**Nome da coluna**: CreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="00034-155">**Column name**: CreatedDateTime</span></span>
      - <span data-ttu-id="00034-156">**Hora de início (UTC)**: selecione uma data antes da data atual</span><span class="sxs-lookup"><span data-stu-id="00034-156">**Start time (UTC)**: select a date sometime prior to the current date</span></span>
      - <span data-ttu-id="00034-157">**Hora de término (UTC)**: selecione a data atual</span><span class="sxs-lookup"><span data-stu-id="00034-157">**End time (UTC)**: select the current date</span></span>
      - <span data-ttu-id="00034-158">Selecione **Importar esquema** na seção _Colunas de_ saída.</span><span class="sxs-lookup"><span data-stu-id="00034-158">Select **Import schema** in the _Output columns_ section.</span></span>

    - <span data-ttu-id="00034-159">Selecione a **atividade Copiar dados** na guia pipeline e selecione a guia **Pia.**</span><span class="sxs-lookup"><span data-stu-id="00034-159">Select the **Copy data** activity in the pipeline tab, then select the **Sink** tab.</span></span>

      - <span data-ttu-id="00034-160">Selecione o **botão Novo,** selecione **Azure Blob Armazenamento** e selecione o **botão Continuar.**</span><span class="sxs-lookup"><span data-stu-id="00034-160">Select the **New** button, select **Azure Blob Storage**, and then select the **Continue** button.</span></span>
      - <span data-ttu-id="00034-161">Selecione **Binário como** o formato dos dados e selecione o botão **Continuar.**</span><span class="sxs-lookup"><span data-stu-id="00034-161">Select **Binary** as the format for the data and then select the **Continue** button.</span></span>
      - <span data-ttu-id="00034-162">Dê ao grupo de dados o nome **M365JsonFile** e crie um novo serviço vinculado se ele ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="00034-162">Give the dataset the name **M365JsonFile** and create new linked service if it does not exist already.</span></span>

    - <span data-ttu-id="00034-163">Na tabela, selecione a guia **Conexão** e selecione **Novo**.</span><span class="sxs-lookup"><span data-stu-id="00034-163">In the table select the **Connection** tab, then select **New**.</span></span>
    - <span data-ttu-id="00034-164">De definir os seguintes valores na caixa de diálogo e selecione **Concluir**.</span><span class="sxs-lookup"><span data-stu-id="00034-164">Set the following values in the dialog, then select **Finish**.</span></span>

        - <span data-ttu-id="00034-165">**Método de autenticação**: Entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="00034-165">**Authentication method**: Service principal</span></span>
        - <span data-ttu-id="00034-166">**Assinatura do Azure**: Selecionar todos</span><span class="sxs-lookup"><span data-stu-id="00034-166">**Azure subscription**: Select all</span></span>
        - <span data-ttu-id="00034-167">**Armazenamento da conta**: mgdcm365datastore</span><span class="sxs-lookup"><span data-stu-id="00034-167">**Storage account name**: mgdcm365datastore</span></span>
          - <span data-ttu-id="00034-168">Essa é a conta de armazenamento criada anteriormente neste exercício.</span><span class="sxs-lookup"><span data-stu-id="00034-168">This is the storage account created earlier in this exercise.</span></span>
        - <span data-ttu-id="00034-169">**Locatário**: insira a ID do locatário do Azure</span><span class="sxs-lookup"><span data-stu-id="00034-169">**Tenant**: enter the ID of your Azure tenant</span></span>
        - <span data-ttu-id="00034-170">**ID da entidade de** serviço : insira a ID do aplicativo do Azure AD que você criou anteriormente</span><span class="sxs-lookup"><span data-stu-id="00034-170">**Service principal ID**: enter the ID of the Azure AD application you previously created</span></span>
        - <span data-ttu-id="00034-171">**Chave de entidade de** serviço : insira a chave de hashed do aplicativo do Azure AD que você criou anteriormente</span><span class="sxs-lookup"><span data-stu-id="00034-171">**Service principal key**: enter the hashed key of the Azure AD application you previously created</span></span>

    - <span data-ttu-id="00034-172">Ao lado do campo **Caminho do arquivo,** selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="00034-172">Next to the **File path** field, select **Browse**.</span></span>
    - <span data-ttu-id="00034-173">Selecione o nome do contêiner de armazenamento criado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="00034-173">Select the name of the storage container you created previously.</span></span>

      ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço de Fábrica de Dados.](images/data-connect-adf-sa-fp-config.png)

1. <span data-ttu-id="00034-176">Com o pipeline criado, selecione o botão **Validar Tudo** na parte superior do designer.</span><span class="sxs-lookup"><span data-stu-id="00034-176">With the pipeline created, select the **Validate All** button at the top of the designer.</span></span>

1. <span data-ttu-id="00034-177">Depois de validar (e corrigir quaisquer problemas encontrados), selecione o botão **Publicar Tudo** na parte superior do designer.</span><span class="sxs-lookup"><span data-stu-id="00034-177">After validating (and fixing any issues that were found), select the **Publish All** button at the top of the designer.</span></span>

## <a name="run-the-azure-data-factory-pipeline"></a><span data-ttu-id="00034-178">Executar o Pipeline da Fábrica de Dados do Azure</span><span class="sxs-lookup"><span data-stu-id="00034-178">Run the Azure Data Factory Pipeline</span></span>

<span data-ttu-id="00034-179">Com o pipeline criado, agora é hora de ser executado.</span><span class="sxs-lookup"><span data-stu-id="00034-179">With the pipeline created, now it is time to run it.</span></span>

> [!NOTE]
> <span data-ttu-id="00034-180">Pode levar vários minutos para que a solicitação de consentimento apareça e não é incomum para todo o processo (iniciar, solicitar consentimento e após aprovar o consentimento concluindo a operação do pipeline) para levar mais de 40 minutos.</span><span class="sxs-lookup"><span data-stu-id="00034-180">It can take several minutes for the consent request to appear and it is not uncommon for the entire process (start, requesting consent and after approving the consent completing the pipeline run) to take over 40 minutes.</span></span>

1. <span data-ttu-id="00034-181">No designer da Fábrica de Dados do Azure, com o pipeline aberto, selecione **Adicionar gatilho > Gatilho Agora**.</span><span class="sxs-lookup"><span data-stu-id="00034-181">In the Azure Data Factory designer, with the pipeline open, select **Add trigger > Trigger Now**.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço Fábrica de Dados para mostrar como ativar um gatilho no pipeline.](images/data-connect-adf-run-trigger.png)

1. <span data-ttu-id="00034-183">Depois de iniciar o trabalho, no menu da barra lateral, selecione **Monitorar** para exibir trabalhos em execução atuais.</span><span class="sxs-lookup"><span data-stu-id="00034-183">After starting the job, from the sidebar menu, select **Monitor** to view current running jobs.</span></span>

1. <span data-ttu-id="00034-184">Na barra de navegação do lado esquerdo, localize a guia **Pipeline runs** e selecione-a.</span><span class="sxs-lookup"><span data-stu-id="00034-184">On the left-side navigation bar, locate the **Pipeline runs** tab and select it.</span></span> <span data-ttu-id="00034-185">Selecione o pipeline na coluna **Nome do pipeline** para exibir o activity **runs**.</span><span class="sxs-lookup"><span data-stu-id="00034-185">Select the pipeline under the **Pipeline name** column to view the **Activity runs**.</span></span> <span data-ttu-id="00034-186">Esse pipeline mostrará como _Em andamento_.</span><span class="sxs-lookup"><span data-stu-id="00034-186">This pipeline will show as _In progress_.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do portal do Azure para a Fábrica de Dados, ela está mostrando a lista de pipelines executados.](images/data-connect-adf-pipeline-runs.png)

1. <span data-ttu-id="00034-188">Depois que você está no **exibição Atividade é executado,** vá para a seção _Atividades_ executados, que está localizada no lado inferior da página.</span><span class="sxs-lookup"><span data-stu-id="00034-188">After you are in the **Activity runs** view, go to the _Activity runs_ section, which is located in the bottom side of the page.</span></span>

1. <span data-ttu-id="00034-189">Passe o mouse sobre **o nome de atividade** e selecione a opção googles.</span><span class="sxs-lookup"><span data-stu-id="00034-189">Hover over the **Activity name** and select the googles option.</span></span> <span data-ttu-id="00034-190">Isso irá trazer a guia **Detalhes.**</span><span class="sxs-lookup"><span data-stu-id="00034-190">This will bring up the **Details** tab.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do Portal do Azure para Data Factory Activity Runs, o usuário está selecionando os googles no nome da atividade para abrir a guia detalhes.](images/data-connect-adf-pipeline-details.png)

1. <span data-ttu-id="00034-192">Na tela **Detalhes,** procure o status da atividade de pipeline como realçada na imagem a seguir.</span><span class="sxs-lookup"><span data-stu-id="00034-192">In the **Details** screen, look for the status of the pipeline activity as highlighted in the following image.</span></span> <span data-ttu-id="00034-193">Nesse caso, você pode ver que ele está em um estado **de RequestingConsent**.</span><span class="sxs-lookup"><span data-stu-id="00034-193">In this case you can see it is in a state of **RequestingConsent**.</span></span>

    ![Uma captura de tela mostrando a interface do usuário do portal do Azure para o serviço de Fábrica de Dados em que o status de carga da solicitação é definido como "RequestConsent".](images/data-connect-adf-wait-for-approval.png)

1. <span data-ttu-id="00034-195">Neste ponto, a atividade é pausada internamente até que alguém aprove manualmente a solicitação de consentimento por meio do Microsoft 365 de administração ou por meio do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="00034-195">At this point, the activity run is internally paused until someone manually approves the consent request via the Microsoft 365 admin center or via PowerShell.</span></span>

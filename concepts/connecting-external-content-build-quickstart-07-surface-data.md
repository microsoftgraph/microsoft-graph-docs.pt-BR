<!-- markdownlint-disable MD002 MD025 MD041 -->

<span data-ttu-id="c6ca1-101">Crie tipos de resultados e verticais de pesquisa para personalizar os resultados da pesquisa no Microsoft SharePoint, Microsoft Office e Pesquisa da Microsoft no Bing, para facilitar a busca das informações que eles têm permissão para ver.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-101">Create search verticals and result types to customize the search results in Microsoft SharePoint, Microsoft Office, and Microsoft Search in Bing, to make it easier for users to find the information that they have permission to see.</span></span>

## <a name="create-a-vertical"></a><span data-ttu-id="c6ca1-102">Criar uma vertical</span><span class="sxs-lookup"><span data-stu-id="c6ca1-102">Create a vertical</span></span>

<span data-ttu-id="c6ca1-103">Para criar e habilitar uma pesquisa vertical no nível da organização, entre no centro de administração do Microsoft 365 usando [a](https://admin.microsoft.com/) função de administrador global e faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c6ca1-103">To create and enable a search vertical at the organization level, sign in to the [Microsoft 365 Admin center](https://admin.microsoft.com/) using the global administrator role, and do the following:</span></span>

1. <span data-ttu-id="c6ca1-104">Vá para **Configurações**  >  **Search & de** inteligência  >  **Personalizações.**</span><span class="sxs-lookup"><span data-stu-id="c6ca1-104">Go to **Settings** > **Search & intelligence** > **Customizations**.</span></span>
2. <span data-ttu-id="c6ca1-105">Vá para **Vertical** e clique no **botão Adicionar.**</span><span class="sxs-lookup"><span data-stu-id="c6ca1-105">Go to **Vertical** and click the **Add** button.</span></span>
3. <span data-ttu-id="c6ca1-106">Forneça os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="c6ca1-106">Provide the following details:</span></span>
  * <span data-ttu-id="c6ca1-107">**Nomeia o vertical:** Partes do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-107">**Name the vertical:** Appliance Parts.</span></span>

   ![Captura de tela da seção "Nome da vertical"](images/connectors-images/build11.png)

  * <span data-ttu-id="c6ca1-109">**Fonte de** conteúdo : o conector criado com o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-109">**Content source**: The connector created with the app.</span></span> <span data-ttu-id="c6ca1-110">(Inventário de Partes)</span><span class="sxs-lookup"><span data-stu-id="c6ca1-110">(Parts Inventory)</span></span>

   ![Captura de tela da seção "Fonte de conteúdo"](images/connectors-images/build12.png)

  * <span data-ttu-id="c6ca1-112">**Adicionar uma consulta**: Deixar em branco.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-112">**Add a query**: Leave blank.</span></span>

   ![Captura de tela da seção "Adicionar uma consulta"](images/connectors-images/build13.png)

  * <span data-ttu-id="c6ca1-114">**Filtros**: Deixar em branco.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-114">**Filters**: Leave blank.</span></span>

   ![Captura de tela da seção "Filters"](images/connectors-images/build14.png)

## <a name="create-a-result-type"></a><span data-ttu-id="c6ca1-116">Criar um tipo de resultado</span><span class="sxs-lookup"><span data-stu-id="c6ca1-116">Create a result type</span></span>

<span data-ttu-id="c6ca1-117">Para criar um tipo de resultado:</span><span class="sxs-lookup"><span data-stu-id="c6ca1-117">To create a result type:</span></span>

1. <span data-ttu-id="c6ca1-118">Vá para **Configurações**  >  **Search & de** inteligência  >  **Personalizações.**</span><span class="sxs-lookup"><span data-stu-id="c6ca1-118">Go to **Settings** > **Search & intelligence** > **Customizations**.</span></span>
2. <span data-ttu-id="c6ca1-119">Vá até a **guia tipo de** resultado e clique no botão **Adicionar.**</span><span class="sxs-lookup"><span data-stu-id="c6ca1-119">Go to the **result type** tab and click the **Add** button.</span></span>
3. <span data-ttu-id="c6ca1-120">Forneça os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="c6ca1-120">Provide the following details:</span></span>

  * <span data-ttu-id="c6ca1-121">**Nome**: Parte do Dispositivo</span><span class="sxs-lookup"><span data-stu-id="c6ca1-121">**Name**: Appliance Part</span></span>

   ![Captura de tela da seção "Nomear o tipo de resultado"](images/connectors-images/build15.png)

  * <span data-ttu-id="c6ca1-123">**Fonte de** conteúdo : o conector criado no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-123">**Content source**: The connector created in the app.</span></span>

   ![Captura de tela da seção "Selecionar uma fonte de conteúdo"](images/connectors-images/build16.png)

  * <span data-ttu-id="c6ca1-125">**Regras**: Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6ca1-125">**Rules**: None</span></span>

   ![Captura de tela da seção "Definir regras"](images/connectors-images/build17.png)

  * <span data-ttu-id="c6ca1-127">Colar o conteúdoresult-type.js[ na](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) caixa de texto do designer de layout.</span><span class="sxs-lookup"><span data-stu-id="c6ca1-127">Paste contents of [result-type.json](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) into the layout designer textbox.</span></span>

   ![Captura de tela da seção "Design layout"](images/connectors-images/build18.png)

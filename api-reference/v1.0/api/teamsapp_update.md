# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="95024-101">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="95024-101">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="95024-102">Atualização de um [aplicativo](../resources/teamsapp.md) publicado anteriormente para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="95024-102">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="95024-103">Essa API especificamente atualiza um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="95024-103">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="95024-104">Para publicar o catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="95024-104">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="95024-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="95024-105">Permissions</span></span>

<span data-ttu-id="95024-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="95024-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="95024-108">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="95024-108">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="95024-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95024-109">Permission Type</span></span>                        | <span data-ttu-id="95024-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95024-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="95024-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95024-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95024-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95024-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="95024-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95024-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95024-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95024-114">Not supported</span></span>|
| <span data-ttu-id="95024-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95024-115">Application</span></span>                            | <span data-ttu-id="95024-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95024-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="95024-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95024-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="95024-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95024-118">Request headers</span></span>

| <span data-ttu-id="95024-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95024-119">Header</span></span>        | <span data-ttu-id="95024-120">Valor</span><span class="sxs-lookup"><span data-stu-id="95024-120">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="95024-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="95024-121">Authorization</span></span> | <span data-ttu-id="95024-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95024-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95024-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95024-124">Content-Type</span></span>  | <span data-ttu-id="95024-125">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="95024-125">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="95024-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95024-126">Request body</span></span>

<span data-ttu-id="95024-127">Carga de manifesto de Zip equipes: Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="95024-127">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="95024-128">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp_list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="95024-128">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="95024-129">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="95024-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="95024-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="95024-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="95024-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95024-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="95024-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95024-132">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="95024-133">Para o aplicativo de equipes zip arquivo, [consulte Criar pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="95024-133">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="95024-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="95024-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

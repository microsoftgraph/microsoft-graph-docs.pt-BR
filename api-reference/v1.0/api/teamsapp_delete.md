# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="41117-101">Remova um aplicativo de catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="41117-101">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="41117-102">Remova o [aplicativo](../resources/teamsapp.md) de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="41117-102">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="41117-103">Para remover o seu aplicativo de catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="41117-103">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="41117-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="41117-104">Permissions</span></span>

<span data-ttu-id="41117-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="41117-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="41117-107">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="41117-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="41117-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41117-108">Permission Type</span></span>                        | <span data-ttu-id="41117-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41117-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="41117-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41117-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="41117-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41117-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="41117-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41117-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41117-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="41117-113">Not supported</span></span>|
| <span data-ttu-id="41117-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41117-114">Application</span></span>                            | <span data-ttu-id="41117-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="41117-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="41117-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41117-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="41117-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41117-117">Request headers</span></span>

| <span data-ttu-id="41117-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41117-118">Header</span></span>        | <span data-ttu-id="41117-119">Valor</span><span class="sxs-lookup"><span data-stu-id="41117-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="41117-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="41117-120">Authorization</span></span> | <span data-ttu-id="41117-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41117-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41117-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41117-123">Request body</span></span>

<span data-ttu-id="41117-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="41117-124">None.</span></span>

><span data-ttu-id="41117-125">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp_list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="41117-125">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="41117-126">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="41117-126">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="41117-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="41117-127">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="41117-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41117-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="41117-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41117-129">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="41117-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="41117-130">Response</span></span>

```http
HTTP/1.1 204 No Content
```

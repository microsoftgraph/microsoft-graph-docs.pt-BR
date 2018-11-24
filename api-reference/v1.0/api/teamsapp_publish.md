# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="71030-101">Publicar aplicativos ao catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="71030-101">Publish apps to your organization's app catalog</span></span>



<span data-ttu-id="71030-102">Publica um [aplicativo](../resources/teamsapp.md) para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="71030-102">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="71030-103">Especificamente, essa API publica o aplicativo catálogo da sua organização (o catálogo de aplicativos do inquilino); o recurso criado terá `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="71030-103">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="71030-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="71030-104">Permissions</span></span>

<span data-ttu-id="71030-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="71030-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="71030-107">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="71030-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="71030-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71030-108">Permission Type</span></span>                        | <span data-ttu-id="71030-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71030-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="71030-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71030-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="71030-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71030-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="71030-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71030-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71030-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="71030-113">Not supported</span></span>|
| <span data-ttu-id="71030-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71030-114">Application</span></span>                            | <span data-ttu-id="71030-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="71030-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="71030-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71030-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="71030-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71030-117">Request headers</span></span>

| <span data-ttu-id="71030-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71030-118">Header</span></span>        | <span data-ttu-id="71030-119">Valor</span><span class="sxs-lookup"><span data-stu-id="71030-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="71030-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="71030-120">Authorization</span></span> | <span data-ttu-id="71030-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71030-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71030-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71030-123">Content-Type</span></span>  | <span data-ttu-id="71030-124">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="71030-124">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="71030-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71030-125">Request body</span></span>

<span data-ttu-id="71030-126">Carga de manifesto de Zip equipes.</span><span class="sxs-lookup"><span data-stu-id="71030-126">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="71030-127">Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="71030-127">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="71030-128">Não é possível criar um aplicativo para uma organização que tem a mesma ID de manifesto do aplicativo outra organização em questão.</span><span class="sxs-lookup"><span data-stu-id="71030-128">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="71030-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="71030-129">Response</span></span>

<span data-ttu-id="71030-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="71030-130">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="71030-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71030-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="71030-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71030-132">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="71030-133">Para obter informações sobre como criar um arquivo do Microsoft Teams aplicativo zip, consulte [criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="71030-133">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="71030-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="71030-134">Response</span></span>

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

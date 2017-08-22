# <a name="list-permissions-on-a-driveitem"></a><span data-ttu-id="0914b-101">Listar permissões em um DriveItem</span><span class="sxs-lookup"><span data-stu-id="0914b-101">List permissions on a DriveItem</span></span>

<span data-ttu-id="0914b-102">Listar as permissões efetivas de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0914b-102">List the effective permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="0914b-p101">A relação **permissions** de um DriveItem não pode ser expandida como parte de uma chamada para [get DriveItem](item_get.md) ou uma coleção de DriveItems. Você deve acessar a propriedade permissions diretamente.</span><span class="sxs-lookup"><span data-stu-id="0914b-p101">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](item_get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="access-to-permissions"></a><span data-ttu-id="0914b-105">Acesso a Permissões</span><span class="sxs-lookup"><span data-stu-id="0914b-105">Access to Permissions</span></span>

<span data-ttu-id="0914b-106">A coleção de permissões inclui informações potencialmente confidenciais e pode não estar disponível para todos os chamadores.</span><span class="sxs-lookup"><span data-stu-id="0914b-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="0914b-p102">Para o proprietário do item, todas as permissões serão retornadas. Isto inclui os coproprietários.</span><span class="sxs-lookup"><span data-stu-id="0914b-p102">For the owner of the item, all permissions will be returned. This includes co-owners.</span></span>
* <span data-ttu-id="0914b-109">Para um chamador não proprietário, somente as permissões que se aplicam ao chamador são retornadas.</span><span class="sxs-lookup"><span data-stu-id="0914b-109">For a non-owner caller, only the permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="0914b-110">Propriedades de permissão que contêm segredos (por exemplo, `shareId` e `webUrl`) são retornadas somente para chamadores que são capazes de criar a permissão.</span><span class="sxs-lookup"><span data-stu-id="0914b-110">Permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the Permission.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0914b-111">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0914b-111">Prerequisites</span></span>
<span data-ttu-id="0914b-112">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0914b-112">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="0914b-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="0914b-113">Files.Read</span></span>
* <span data-ttu-id="0914b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0914b-114">Files.ReadWrite</span></span>
* <span data-ttu-id="0914b-115">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="0914b-115">Files.Read.All</span></span>
* <span data-ttu-id="0914b-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0914b-116">Files.ReadWrite.All</span></span>
* <span data-ttu-id="0914b-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="0914b-117">Sites.Read.All</span></span>
* <span data-ttu-id="0914b-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0914b-118">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0914b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0914b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="0914b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0914b-120">Request headers</span></span>

| <span data-ttu-id="0914b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0914b-121">Name</span></span>          | <span data-ttu-id="0914b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0914b-122">Type</span></span>   | <span data-ttu-id="0914b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0914b-123">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0914b-124">if-none-match</span><span class="sxs-lookup"><span data-stu-id="0914b-124">if-none-match</span></span> | <span data-ttu-id="0914b-125">string</span><span class="sxs-lookup"><span data-stu-id="0914b-125">string</span></span> | <span data-ttu-id="0914b-126">Se este cabeçalho de solicitação estiver incluso e a etag fornecida corresponder à marca atual do item, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="0914b-126">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="optional-query-parameters"></a><span data-ttu-id="0914b-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0914b-127">Optional query parameters</span></span>
<span data-ttu-id="0914b-128">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0914b-128">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="0914b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0914b-129">Request body</span></span>
<span data-ttu-id="0914b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0914b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0914b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0914b-131">Response</span></span>

<span data-ttu-id="0914b-132">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0914b-132">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="0914b-133">As permissões efetivas de um item podem se originar de duas fontes:</span><span class="sxs-lookup"><span data-stu-id="0914b-133">Effective permissions of an item can come from two sources:</span></span>

* <span data-ttu-id="0914b-134">Permissões aplicadas diretamente ao próprio item</span><span class="sxs-lookup"><span data-stu-id="0914b-134">Permissions applied directly on the item itself</span></span>
* <span data-ttu-id="0914b-135">Permissões herdadas de ancestrais do item</span><span class="sxs-lookup"><span data-stu-id="0914b-135">Permissions inherited from the item's ancestors</span></span>

<span data-ttu-id="0914b-p103">Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade **inheritedFrom**. Esta propriedade é um recurso [**itemReference**](../resources/itemreference.md) que referencia o ancestral do qual a permissão é herdada.</span><span class="sxs-lookup"><span data-stu-id="0914b-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="0914b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0914b-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0914b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0914b-139">Request</span></span>
<span data-ttu-id="0914b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0914b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a><span data-ttu-id="0914b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0914b-141">Response</span></span>
<span data-ttu-id="0914b-142">Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0914b-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

<span data-ttu-id="0914b-143">Veja [Obter permissão](permission_get.md) para obter mais detalhes sobre como recuperar um recurso de permissão única.</span><span class="sxs-lookup"><span data-stu-id="0914b-143">See [Get permission](permission_get.md) for more details on retrieving a single permission resource.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->

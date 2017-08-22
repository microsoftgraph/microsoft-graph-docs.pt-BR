# <a name="get-permission"></a><span data-ttu-id="a1997-101">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="a1997-101">Get permission</span></span>

<span data-ttu-id="a1997-102">Recupere as propriedades e os relacionamentos do objeto permission.</span><span class="sxs-lookup"><span data-stu-id="a1997-102">Retrieve the properties and relationships of permission object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1997-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1997-103">Prerequisites</span></span>
<span data-ttu-id="a1997-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="a1997-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="a1997-105">Files.Read</span><span class="sxs-lookup"><span data-stu-id="a1997-105">Files.Read</span></span>
* <span data-ttu-id="a1997-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1997-106">Files.ReadWrite</span></span>
* <span data-ttu-id="a1997-107">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1997-107">Files.Read.All</span></span>
* <span data-ttu-id="a1997-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1997-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="a1997-109">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1997-109">Sites.Read.All</span></span>
* <span data-ttu-id="a1997-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1997-110">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a1997-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1997-111">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/root:/{path}:/permissions/{perm-id}
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1997-112">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1997-112">Optional query parameters</span></span>
<span data-ttu-id="a1997-113">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1997-113">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="a1997-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1997-114">Request body</span></span>
<span data-ttu-id="a1997-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1997-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1997-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1997-116">Response</span></span>

<span data-ttu-id="a1997-117">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1997-117">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1997-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1997-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a1997-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1997-119">Request</span></span>

<span data-ttu-id="a1997-120">Aqui está um exemplo da solicitação para acessar uma permissão na pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="a1997-120">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_permission"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
```
##### <a name="response"></a><span data-ttu-id="a1997-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1997-121">Response</span></span>
<span data-ttu-id="a1997-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1997-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 762

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="a1997-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a1997-123">Remarks</span></span>

<span data-ttu-id="a1997-124">O recurso [Permission](../resources/permission.md) usa _facets_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="a1997-124">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="a1997-p101">Permissões com uma faceta [**link**](../resources/sharinglink.md) representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="a1997-p101">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="a1997-127">Permissões com uma faceta [**invitation**](../resources/sharinginvitation.md) representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="a1997-127">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->

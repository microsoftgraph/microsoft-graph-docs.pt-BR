# <a name="get-permission"></a><span data-ttu-id="78e4f-101">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="78e4f-101">Get permission</span></span>

<span data-ttu-id="78e4f-102">Recuperar as propriedades e os relacionamentos do objeto permission.</span><span class="sxs-lookup"><span data-stu-id="78e4f-102">Retrieve the properties and relationships of permission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="78e4f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="78e4f-103">Permissions</span></span>
<span data-ttu-id="78e4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="78e4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78e4f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78e4f-106">Permission type</span></span>      | <span data-ttu-id="78e4f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78e4f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="78e4f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78e4f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="78e4f-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e4f-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="78e4f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78e4f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78e4f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e4f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="78e4f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78e4f-112">Application</span></span> | <span data-ttu-id="78e4f-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e4f-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="78e4f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78e4f-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/root:/{path}:/permissions/{perm-id}
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78e4f-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78e4f-115">Optional query parameters</span></span>
<span data-ttu-id="78e4f-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78e4f-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="78e4f-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78e4f-117">Request body</span></span>
<span data-ttu-id="78e4f-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78e4f-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78e4f-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e4f-119">Response</span></span>

<span data-ttu-id="78e4f-120">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78e4f-120">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e4f-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78e4f-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="78e4f-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78e4f-122">Request</span></span>

<span data-ttu-id="78e4f-123">Aqui está um exemplo da solicitação para acessar uma permissão na pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="78e4f-123">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_permission"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
```
##### <a name="response"></a><span data-ttu-id="78e4f-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e4f-124">Response</span></span>
<span data-ttu-id="78e4f-125">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78e4f-125">Here is an example of the response.</span></span>
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

## <a name="remarks"></a><span data-ttu-id="78e4f-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="78e4f-126">Remarks</span></span>

<span data-ttu-id="78e4f-127">O recurso [Permission](../resources/permission.md) usa _facets_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="78e4f-127">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="78e4f-p102">Permissões com uma faceta [**link**](../resources/sharinglink.md) representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="78e4f-p102">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="78e4f-130">Permissões com uma faceta [**invitation**](../resources/sharinginvitation.md) representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="78e4f-130">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->

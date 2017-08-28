# <a name="get-a-driveitem-resource"></a><span data-ttu-id="4e9ec-101">Obter um recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="4e9ec-101">Get a DriveItem resource</span></span>

<span data-ttu-id="4e9ec-102">Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e9ec-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e9ec-103">Permissions</span></span>
<span data-ttu-id="4e9ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e9ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4e9ec-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e9ec-106">Permission type</span></span>      | <span data-ttu-id="4e9ec-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e9ec-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4e9ec-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e9ec-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4e9ec-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9ec-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4e9ec-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e9ec-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e9ec-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9ec-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4e9ec-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e9ec-112">Application</span></span> | <span data-ttu-id="4e9ec-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9ec-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4e9ec-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e9ec-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e9ec-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4e9ec-115">Optional query parameters</span></span>
<span data-ttu-id="4e9ec-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e9ec-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e9ec-117">Request headers</span></span>

| <span data-ttu-id="4e9ec-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4e9ec-118">Name</span></span>          | <span data-ttu-id="4e9ec-119">Valor</span><span class="sxs-lookup"><span data-stu-id="4e9ec-119">Value</span></span>  | <span data-ttu-id="4e9ec-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e9ec-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4e9ec-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="4e9ec-121">if-none-match</span></span> | <span data-ttu-id="4e9ec-122">String</span><span class="sxs-lookup"><span data-stu-id="4e9ec-122">String</span></span> | <span data-ttu-id="4e9ec-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4e9ec-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e9ec-124">Request body</span></span>
<span data-ttu-id="4e9ec-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e9ec-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e9ec-126">Response</span></span>

<span data-ttu-id="4e9ec-127">Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e9ec-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e9ec-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4e9ec-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e9ec-129">Request</span></span>

<span data-ttu-id="4e9ec-130">Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <a name="response"></a><span data-ttu-id="4e9ec-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e9ec-131">Response</span></span>
<span data-ttu-id="4e9ec-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-132">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="notes"></a><span data-ttu-id="4e9ec-133">Observações</span><span class="sxs-lookup"><span data-stu-id="4e9ec-133">Notes</span></span>

<span data-ttu-id="4e9ec-134">É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.</span><span class="sxs-lookup"><span data-stu-id="4e9ec-134">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->

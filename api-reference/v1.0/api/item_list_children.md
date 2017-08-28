# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="4f8fd-101">Listar os filhos de um driveItem</span><span class="sxs-lookup"><span data-stu-id="4f8fd-101">List children of a driveItem</span></span>

<span data-ttu-id="4f8fd-102">Retorne uma coleção de [DriveItems](../resources/driveitem.md) na relação **children** de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="4f8fd-103">DriveItems com uma faceta **folder** ou **package** não nula podem ter um ou mais DriveItems filhos.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="4f8fd-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f8fd-104">Permissions</span></span>
<span data-ttu-id="4f8fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f8fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f8fd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f8fd-107">Permission type</span></span>      | <span data-ttu-id="4f8fd-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f8fd-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4f8fd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f8fd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4f8fd-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f8fd-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4f8fd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f8fd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f8fd-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f8fd-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4f8fd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f8fd-113">Application</span></span> | <span data-ttu-id="4f8fd-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f8fd-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4f8fd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f8fd-115">HTTP request</span></span>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f8fd-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f8fd-116">Optional query parameters</span></span>
<span data-ttu-id="4f8fd-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f8fd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f8fd-118">Request headers</span></span>

| <span data-ttu-id="4f8fd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4f8fd-119">Name</span></span>          | <span data-ttu-id="4f8fd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f8fd-120">Type</span></span>   | <span data-ttu-id="4f8fd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f8fd-121">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f8fd-122">if-none-match</span><span class="sxs-lookup"><span data-stu-id="4f8fd-122">if-none-match</span></span> | <span data-ttu-id="4f8fd-123">String</span><span class="sxs-lookup"><span data-stu-id="4f8fd-123">String</span></span> | <span data-ttu-id="4f8fd-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-124">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f8fd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f8fd-125">Request body</span></span>
<span data-ttu-id="4f8fd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-126">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="4f8fd-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f8fd-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4f8fd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f8fd-128">Request</span></span>
<span data-ttu-id="4f8fd-129">Aqui está um exemplo da solicitação para retornar DriveItems na pasta raiz do OneDrive do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-129">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a><span data-ttu-id="4f8fd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f8fd-130">Response</span></span>

<span data-ttu-id="4f8fd-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="4f8fd-132">**Observação:** Se uma coleção exceder o tamanho de página padrão (200 itens), a propriedade **@odata.nextLink** será retornada na resposta para indicar que mais itens estão disponíveis e fornecer a URL da solicitação para a próxima página de itens.</span><span class="sxs-lookup"><span data-stu-id="4f8fd-132">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="4f8fd-133">Você pode controlar o tamanho da página por meio de [parâmetros de cadeia de caracteres de consulta opcional](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="4f8fd-133">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->

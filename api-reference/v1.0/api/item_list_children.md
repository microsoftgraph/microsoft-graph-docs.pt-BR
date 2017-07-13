# <span data-ttu-id="f0711-101">Listar os filhos de um driveItem</span><span class="sxs-lookup"><span data-stu-id="f0711-101">List children of a driveItem</span></span>
<a id="list-children-of-a-driveitem" class="xliff"></a>

<span data-ttu-id="f0711-102">Retorne uma coleção de [DriveItems](../resources/driveitem.md) na relação **children** de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="f0711-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="f0711-103">DriveItems com uma faceta **folder** ou **package** não nula podem ter um ou mais DriveItems filhos.</span><span class="sxs-lookup"><span data-stu-id="f0711-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <span data-ttu-id="f0711-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0711-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="f0711-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="f0711-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="f0711-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="f0711-106">Files.Read</span></span>
* <span data-ttu-id="f0711-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0711-107">Files.ReadWrite</span></span>
* <span data-ttu-id="f0711-108">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0711-108">Files.Read.All</span></span>
* <span data-ttu-id="f0711-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0711-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="f0711-110">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0711-110">Sites.Read.All</span></span>
* <span data-ttu-id="f0711-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0711-111">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="f0711-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0711-112">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="f0711-113">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0711-113">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="f0711-114">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0711-114">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="f0711-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0711-115">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="f0711-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f0711-116">Name</span></span>          | <span data-ttu-id="f0711-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0711-117">Type</span></span>   | <span data-ttu-id="f0711-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0711-118">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f0711-119">if-none-match</span><span class="sxs-lookup"><span data-stu-id="f0711-119">if-none-match</span></span> | <span data-ttu-id="f0711-120">String</span><span class="sxs-lookup"><span data-stu-id="f0711-120">String</span></span> | <span data-ttu-id="f0711-121">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="f0711-121">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <span data-ttu-id="f0711-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0711-122">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="f0711-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0711-123">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="f0711-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0711-124">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="f0711-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0711-125">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f0711-126">Aqui está um exemplo da solicitação para retornar DriveItems na pasta raiz do OneDrive do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="f0711-126">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <span data-ttu-id="f0711-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0711-127">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="f0711-128">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0711-128">Here is an example of the response.</span></span>
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

<span data-ttu-id="f0711-129">**Observação:** Se uma coleção exceder o tamanho de página padrão (200 itens), a propriedade **@odata.nextLink** será retornada na resposta para indicar que mais itens estão disponíveis e fornecer a URL da solicitação para a próxima página de itens.</span><span class="sxs-lookup"><span data-stu-id="f0711-129">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="f0711-130">Você pode controlar o tamanho da página por meio de [parâmetros de cadeia de caracteres de consulta opcional](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="f0711-130">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->

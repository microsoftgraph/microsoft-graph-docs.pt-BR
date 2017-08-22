# <a name="get-page"></a><span data-ttu-id="768ff-101">Get page</span><span class="sxs-lookup"><span data-stu-id="768ff-101">Get page</span></span>

<span data-ttu-id="768ff-102">Recupere as propriedades e os relacionamentos de um objeto [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="768ff-102">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="768ff-103">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="768ff-103">**Getting page information**</span></span>

<span data-ttu-id="768ff-104">Acesse os metadados de uma página pelo identificador da página:</span><span class="sxs-lookup"><span data-stu-id="768ff-104">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="768ff-105">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="768ff-105">**Getting page content**</span></span>

<span data-ttu-id="768ff-106">Você pode usar o ponto de extremidade `content` da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="768ff-106">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="768ff-107">A opção de consulta `includeIDs=true` é usada para [atualizar páginas](../api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="768ff-107">The `includeIDs=true` query option is used to [update pages](../api/page_update.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="768ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="768ff-108">Prerequisites</span></span>
<span data-ttu-id="768ff-109">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="768ff-109">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="768ff-110">Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="768ff-110">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="768ff-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="768ff-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="768ff-112">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="768ff-112">Optional query parameters</span></span>
<span data-ttu-id="768ff-113">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="768ff-113">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="768ff-p101">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="768ff-p101">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="768ff-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="768ff-116">Request headers</span></span>
| <span data-ttu-id="768ff-117">Nome</span><span class="sxs-lookup"><span data-stu-id="768ff-117">Name</span></span>       | <span data-ttu-id="768ff-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="768ff-118">Type</span></span> | <span data-ttu-id="768ff-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="768ff-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="768ff-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="768ff-120">Authorization</span></span>  | <span data-ttu-id="768ff-121">string</span><span class="sxs-lookup"><span data-stu-id="768ff-121">string</span></span>  | <span data-ttu-id="768ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="768ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="768ff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="768ff-124">Accept</span></span> | <span data-ttu-id="768ff-125">string</span><span class="sxs-lookup"><span data-stu-id="768ff-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="768ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="768ff-126">Request body</span></span>
<span data-ttu-id="768ff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="768ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="768ff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="768ff-128">Response</span></span>

<span data-ttu-id="768ff-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="768ff-129">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="768ff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="768ff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="768ff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="768ff-131">Request</span></span>
<span data-ttu-id="768ff-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="768ff-132">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="768ff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="768ff-133">Response</span></span>
<span data-ttu-id="768ff-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="768ff-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

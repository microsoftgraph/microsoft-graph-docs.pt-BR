# <a name="list-pages"></a><span data-ttu-id="79330-101">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="79330-101">List pages</span></span>

<span data-ttu-id="79330-102">Recupere uma lista de objetos [page](../resources/page.md) da seção especificada.</span><span class="sxs-lookup"><span data-stu-id="79330-102">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79330-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79330-103">Prerequisites</span></span>
<span data-ttu-id="79330-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="79330-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="79330-105">Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79330-105">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="79330-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79330-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79330-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79330-107">Optional query parameters</span></span>
<span data-ttu-id="79330-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79330-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="79330-p101">A consulta padrão das páginas retorna as 20 páginas principais ordenadas por `lastModifiedTime desc`. Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para passar pelo conjunto de resultados. o número máximo de páginas retornadas em uma solicitação `top` é 100.</span><span class="sxs-lookup"><span data-stu-id="79330-p101">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="79330-p102">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="79330-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79330-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79330-114">Request headers</span></span>
| <span data-ttu-id="79330-115">Nome</span><span class="sxs-lookup"><span data-stu-id="79330-115">Name</span></span>       | <span data-ttu-id="79330-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="79330-116">Type</span></span> | <span data-ttu-id="79330-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="79330-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="79330-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="79330-118">Authorization</span></span>  | <span data-ttu-id="79330-119">string</span><span class="sxs-lookup"><span data-stu-id="79330-119">string</span></span>  | <span data-ttu-id="79330-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79330-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79330-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79330-122">Accept</span></span> | <span data-ttu-id="79330-123">string</span><span class="sxs-lookup"><span data-stu-id="79330-123">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="79330-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79330-124">Request body</span></span>
<span data-ttu-id="79330-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79330-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79330-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="79330-126">Response</span></span>

<span data-ttu-id="79330-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79330-127">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79330-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79330-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79330-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79330-129">Request</span></span>
<span data-ttu-id="79330-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79330-130">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="79330-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="79330-131">Response</span></span>
<span data-ttu-id="79330-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79330-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
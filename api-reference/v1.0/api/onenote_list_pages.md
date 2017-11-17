# <a name="list-pages"></a><span data-ttu-id="81448-101">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="81448-101">List pages</span></span>

<span data-ttu-id="81448-102">Recuperar uma lista de objetos [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="81448-102">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="81448-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="81448-103">Permissions</span></span>
<span data-ttu-id="81448-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81448-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81448-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81448-106">Permission type</span></span>      | <span data-ttu-id="81448-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81448-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81448-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81448-108">Delegated (work or school account)</span></span> | <span data-ttu-id="81448-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81448-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="81448-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81448-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81448-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81448-111">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="81448-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81448-112">Application</span></span> | <span data-ttu-id="81448-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81448-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81448-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81448-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81448-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81448-115">Optional query parameters</span></span>
<span data-ttu-id="81448-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81448-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="81448-p102">A consulta padrão das páginas retorna as 20 páginas principais ordenadas por `lastModifiedTime desc`. Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para passar pelo conjunto de resultados. o número máximo de páginas retornadas em uma solicitação `top` é 100.</span><span class="sxs-lookup"><span data-stu-id="81448-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="81448-p103">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `displayName` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="81448-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81448-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81448-122">Request headers</span></span>
| <span data-ttu-id="81448-123">Nome</span><span class="sxs-lookup"><span data-stu-id="81448-123">Name</span></span>       | <span data-ttu-id="81448-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="81448-124">Type</span></span> | <span data-ttu-id="81448-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="81448-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81448-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="81448-126">Authorization</span></span>  | <span data-ttu-id="81448-127">string</span><span class="sxs-lookup"><span data-stu-id="81448-127">string</span></span>  | <span data-ttu-id="81448-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81448-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81448-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81448-130">Accept</span></span> | <span data-ttu-id="81448-131">string</span><span class="sxs-lookup"><span data-stu-id="81448-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="81448-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81448-132">Request body</span></span>
<span data-ttu-id="81448-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81448-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81448-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="81448-134">Response</span></span>

<span data-ttu-id="81448-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81448-135">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81448-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81448-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81448-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81448-137">Request</span></span>
<span data-ttu-id="81448-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81448-138">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="81448-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="81448-139">Response</span></span>
<span data-ttu-id="81448-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81448-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
# <a name="get-page"></a><span data-ttu-id="f0643-101">Get page</span><span class="sxs-lookup"><span data-stu-id="f0643-101">Get page</span></span>

<span data-ttu-id="f0643-102">Recupere as propriedades e os relacionamentos de um objeto [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="f0643-102">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="f0643-103">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="f0643-103">**Getting page information**</span></span>

<span data-ttu-id="f0643-104">Acesse os metadados de uma página pelo identificador da página:</span><span class="sxs-lookup"><span data-stu-id="f0643-104">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="f0643-105">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="f0643-105">**Getting page content**</span></span>

<span data-ttu-id="f0643-106">Você pode usar o ponto de extremidade `content` da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="f0643-106">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="f0643-107">A opção de consulta `includeIDs=true` é usada para [atualizar páginas](../api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="f0643-107">The `includeIDs=true` query option is used to [update pages](../api/page_update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0643-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0643-108">Permissions</span></span>
<span data-ttu-id="f0643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0643-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0643-111">Permission type</span></span>      | <span data-ttu-id="f0643-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0643-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f0643-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0643-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f0643-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0643-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f0643-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0643-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0643-116">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0643-116">Notes.Read, Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="f0643-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0643-117">Application</span></span> | <span data-ttu-id="f0643-118">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0643-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f0643-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0643-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0643-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0643-120">Optional query parameters</span></span>
<span data-ttu-id="f0643-121">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0643-121">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f0643-p102">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="f0643-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0643-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0643-124">Request headers</span></span>
| <span data-ttu-id="f0643-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f0643-125">Name</span></span>       | <span data-ttu-id="f0643-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0643-126">Type</span></span> | <span data-ttu-id="f0643-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0643-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0643-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0643-128">Authorization</span></span>  | <span data-ttu-id="f0643-129">string</span><span class="sxs-lookup"><span data-stu-id="f0643-129">string</span></span>  | <span data-ttu-id="f0643-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0643-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0643-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0643-132">Accept</span></span> | <span data-ttu-id="f0643-133">string</span><span class="sxs-lookup"><span data-stu-id="f0643-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f0643-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0643-134">Request body</span></span>
<span data-ttu-id="f0643-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0643-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0643-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0643-136">Response</span></span>

<span data-ttu-id="f0643-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0643-137">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0643-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0643-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0643-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0643-139">Request</span></span>
<span data-ttu-id="f0643-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0643-140">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="f0643-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0643-141">Response</span></span>
<span data-ttu-id="f0643-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0643-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

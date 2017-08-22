# <a name="get-notebook"></a><span data-ttu-id="45a51-101">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="45a51-101">Get notebook</span></span>

<span data-ttu-id="45a51-102">Recupere as propriedades e os relacionamentos de um objeto [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="45a51-102">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45a51-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45a51-103">Prerequisites</span></span>
<span data-ttu-id="45a51-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="45a51-104">One of the following **scopes** is required to execute this API:</span></span>
  
<span data-ttu-id="45a51-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a51-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="45a51-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a51-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45a51-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45a51-107">Optional query parameters</span></span>
<span data-ttu-id="45a51-108">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45a51-108">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="45a51-109">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="45a51-109">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45a51-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a51-110">Request headers</span></span>
| <span data-ttu-id="45a51-111">Nome</span><span class="sxs-lookup"><span data-stu-id="45a51-111">Name</span></span>       | <span data-ttu-id="45a51-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a51-112">Type</span></span> | <span data-ttu-id="45a51-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a51-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45a51-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a51-114">Authorization</span></span>  | <span data-ttu-id="45a51-115">string</span><span class="sxs-lookup"><span data-stu-id="45a51-115">string</span></span>  | <span data-ttu-id="45a51-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a51-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45a51-118">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45a51-118">Accept</span></span> | <span data-ttu-id="45a51-119">string</span><span class="sxs-lookup"><span data-stu-id="45a51-119">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="45a51-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45a51-120">Request body</span></span>
<span data-ttu-id="45a51-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45a51-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45a51-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a51-122">Response</span></span>

<span data-ttu-id="45a51-123">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45a51-123">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45a51-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45a51-124">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45a51-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a51-125">Request</span></span>
<span data-ttu-id="45a51-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45a51-126">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="45a51-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a51-127">Response</span></span>
<span data-ttu-id="45a51-p102">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45a51-p102">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

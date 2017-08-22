# <a name="get-section"></a><span data-ttu-id="f5834-101">Obter seção</span><span class="sxs-lookup"><span data-stu-id="f5834-101">Get section</span></span>

<span data-ttu-id="f5834-102">Recupere as propriedades e os relacionamentos de um objeto [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="f5834-102">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5834-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5834-103">Prerequisites</span></span>
<span data-ttu-id="f5834-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="f5834-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="f5834-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5834-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="f5834-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5834-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5834-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5834-107">Optional query parameters</span></span>
<span data-ttu-id="f5834-108">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5834-108">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f5834-p101">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="f5834-p101">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5834-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5834-111">Request headers</span></span>
| <span data-ttu-id="f5834-112">Nome</span><span class="sxs-lookup"><span data-stu-id="f5834-112">Name</span></span>       | <span data-ttu-id="f5834-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5834-113">Type</span></span> | <span data-ttu-id="f5834-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5834-114">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5834-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5834-115">Authorization</span></span>  | <span data-ttu-id="f5834-116">string</span><span class="sxs-lookup"><span data-stu-id="f5834-116">string</span></span>  | <span data-ttu-id="f5834-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5834-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5834-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5834-119">Accept</span></span> | <span data-ttu-id="f5834-120">string</span><span class="sxs-lookup"><span data-stu-id="f5834-120">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="f5834-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5834-121">Request body</span></span>
<span data-ttu-id="f5834-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5834-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5834-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5834-123">Response</span></span>

<span data-ttu-id="f5834-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5834-124">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5834-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5834-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5834-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5834-126">Request</span></span>
<span data-ttu-id="f5834-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5834-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="f5834-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5834-128">Response</span></span>
<span data-ttu-id="f5834-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5834-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
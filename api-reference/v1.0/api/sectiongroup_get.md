# <a name="get-sectiongroup"></a><span data-ttu-id="c5672-101">Obter sectionGroup</span><span class="sxs-lookup"><span data-stu-id="c5672-101">Get sectionGroup</span></span>

<span data-ttu-id="c5672-102">Recupere as propriedades e os relacionamentos de um objeto [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="c5672-102">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5672-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5672-103">Prerequisites</span></span>
<span data-ttu-id="c5672-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="c5672-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="c5672-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5672-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c5672-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5672-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5672-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5672-107">Optional query parameters</span></span>
<span data-ttu-id="c5672-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5672-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c5672-p101">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `name` e `self`. Os valores `expand` válidos para o grupo de seção são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="c5672-p101">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5672-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5672-111">Request headers</span></span>
| <span data-ttu-id="c5672-112">Nome</span><span class="sxs-lookup"><span data-stu-id="c5672-112">Name</span></span>       | <span data-ttu-id="c5672-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5672-113">Type</span></span> | <span data-ttu-id="c5672-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5672-114">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5672-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5672-115">Authorization</span></span>  | <span data-ttu-id="c5672-116">string</span><span class="sxs-lookup"><span data-stu-id="c5672-116">string</span></span>  | <span data-ttu-id="c5672-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5672-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5672-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5672-119">Accept</span></span> | <span data-ttu-id="c5672-120">string</span><span class="sxs-lookup"><span data-stu-id="c5672-120">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="c5672-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5672-121">Request body</span></span>
<span data-ttu-id="c5672-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5672-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5672-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5672-123">Response</span></span>

<span data-ttu-id="c5672-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5672-124">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5672-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5672-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5672-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5672-126">Request</span></span>
<span data-ttu-id="c5672-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5672-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="c5672-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5672-128">Response</span></span>
<span data-ttu-id="c5672-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5672-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
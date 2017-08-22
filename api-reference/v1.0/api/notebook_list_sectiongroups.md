# <a name="list-sectiongroups"></a><span data-ttu-id="36fdb-101">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="36fdb-101">List sectionGroups</span></span>

<span data-ttu-id="36fdb-102">Recupere uma lista de objetos [section groups](../resources/sectiongroup.md) do bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="36fdb-102">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36fdb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36fdb-103">Prerequisites</span></span>
<span data-ttu-id="36fdb-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="36fdb-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="36fdb-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36fdb-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="36fdb-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36fdb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36fdb-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36fdb-107">Optional query parameters</span></span>
<span data-ttu-id="36fdb-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36fdb-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="36fdb-109">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="36fdb-109">The default sort order is `name asc`.</span></span>

<span data-ttu-id="36fdb-p101">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `sections`, `sectionGroups`, `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="36fdb-p101">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36fdb-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36fdb-112">Request headers</span></span>
| <span data-ttu-id="36fdb-113">Nome</span><span class="sxs-lookup"><span data-stu-id="36fdb-113">Name</span></span>       | <span data-ttu-id="36fdb-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="36fdb-114">Type</span></span> | <span data-ttu-id="36fdb-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="36fdb-115">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36fdb-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="36fdb-116">Authorization</span></span>  | <span data-ttu-id="36fdb-117">string</span><span class="sxs-lookup"><span data-stu-id="36fdb-117">string</span></span>  | <span data-ttu-id="36fdb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36fdb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36fdb-120">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36fdb-120">Accept</span></span> | <span data-ttu-id="36fdb-121">string</span><span class="sxs-lookup"><span data-stu-id="36fdb-121">string</span></span> | `application/json` |  

## <a name="request-body"></a><span data-ttu-id="36fdb-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36fdb-122">Request body</span></span>
<span data-ttu-id="36fdb-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36fdb-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36fdb-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="36fdb-124">Response</span></span>

<span data-ttu-id="36fdb-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36fdb-125">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36fdb-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36fdb-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36fdb-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36fdb-127">Request</span></span>
<span data-ttu-id="36fdb-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36fdb-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="36fdb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="36fdb-129">Response</span></span>
<span data-ttu-id="36fdb-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36fdb-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

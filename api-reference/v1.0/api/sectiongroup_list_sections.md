# <a name="list-sections"></a><span data-ttu-id="380c4-101">Listar seções</span><span class="sxs-lookup"><span data-stu-id="380c4-101">List sections</span></span>

<span data-ttu-id="380c4-102">Recupere uma lista de objetos [section](../resources/section.md) do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="380c4-102">Retrieve a list of [section](../resources/section.md) objects from the specified section group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="380c4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="380c4-103">Prerequisites</span></span>
<span data-ttu-id="380c4-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="380c4-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="380c4-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="380c4-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="380c4-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="380c4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="380c4-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="380c4-107">Optional query parameters</span></span>
<span data-ttu-id="380c4-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="380c4-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="380c4-109">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="380c4-109">The default sort order is `name asc`.</span></span>

<span data-ttu-id="380c4-p101">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="380c4-p101">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="380c4-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="380c4-112">Request headers</span></span>
| <span data-ttu-id="380c4-113">Nome</span><span class="sxs-lookup"><span data-stu-id="380c4-113">Name</span></span>       | <span data-ttu-id="380c4-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="380c4-114">Type</span></span> | <span data-ttu-id="380c4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="380c4-115">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="380c4-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="380c4-116">Authorization</span></span>  | <span data-ttu-id="380c4-117">string</span><span class="sxs-lookup"><span data-stu-id="380c4-117">string</span></span>  | <span data-ttu-id="380c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="380c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="380c4-120">Aceitar</span><span class="sxs-lookup"><span data-stu-id="380c4-120">Accept</span></span> | <span data-ttu-id="380c4-121">string</span><span class="sxs-lookup"><span data-stu-id="380c4-121">string</span></span> | `application/json` |  

## <a name="request-body"></a><span data-ttu-id="380c4-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="380c4-122">Request body</span></span>
<span data-ttu-id="380c4-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="380c4-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="380c4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="380c4-124">Response</span></span>

<span data-ttu-id="380c4-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="380c4-125">If successful, this method returns a `200 OK` response code and a collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="380c4-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="380c4-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="380c4-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="380c4-127">Request</span></span>
<span data-ttu-id="380c4-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="380c4-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="380c4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="380c4-129">Response</span></span>
<span data-ttu-id="380c4-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="380c4-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
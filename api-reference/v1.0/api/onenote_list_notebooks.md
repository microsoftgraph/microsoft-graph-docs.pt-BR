# <a name="list-notebooks"></a><span data-ttu-id="d403b-101">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="d403b-101">List notebooks</span></span>

<span data-ttu-id="d403b-102">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="d403b-102">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d403b-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d403b-103">Prerequisites</span></span>
<span data-ttu-id="d403b-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="d403b-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="d403b-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d403b-105">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="d403b-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d403b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d403b-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d403b-107">Optional query parameters</span></span>
<span data-ttu-id="d403b-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d403b-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d403b-109">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="d403b-109">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="d403b-110">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="d403b-110">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d403b-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d403b-111">Request headers</span></span>
| <span data-ttu-id="d403b-112">Nome</span><span class="sxs-lookup"><span data-stu-id="d403b-112">Name</span></span>       | <span data-ttu-id="d403b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="d403b-113">Type</span></span> | <span data-ttu-id="d403b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d403b-114">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d403b-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="d403b-115">Authorization</span></span>  | <span data-ttu-id="d403b-116">string</span><span class="sxs-lookup"><span data-stu-id="d403b-116">string</span></span>  | <span data-ttu-id="d403b-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d403b-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d403b-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d403b-119">Accept</span></span> | <span data-ttu-id="d403b-120">string</span><span class="sxs-lookup"><span data-stu-id="d403b-120">string</span></span> | `application/json` |  

## <a name="request-body"></a><span data-ttu-id="d403b-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d403b-121">Request body</span></span>
<span data-ttu-id="d403b-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d403b-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d403b-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="d403b-123">Response</span></span>

<span data-ttu-id="d403b-124">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d403b-124">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d403b-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d403b-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d403b-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d403b-126">Request</span></span>
<span data-ttu-id="d403b-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d403b-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="d403b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d403b-128">Response</span></span>
<span data-ttu-id="d403b-p102">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d403b-p102">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
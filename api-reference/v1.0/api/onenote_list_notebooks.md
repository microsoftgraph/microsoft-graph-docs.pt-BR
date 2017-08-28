# <a name="list-notebooks"></a><span data-ttu-id="1621a-101">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="1621a-101">List notebooks</span></span>

<span data-ttu-id="1621a-102">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="1621a-102">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1621a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1621a-103">Permissions</span></span>
<span data-ttu-id="1621a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1621a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1621a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1621a-106">Permission type</span></span>      | <span data-ttu-id="1621a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1621a-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1621a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1621a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1621a-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1621a-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="1621a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1621a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1621a-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1621a-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="1621a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1621a-112">Application</span></span> | <span data-ttu-id="1621a-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1621a-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1621a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1621a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1621a-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1621a-115">Optional query parameters</span></span>
<span data-ttu-id="1621a-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1621a-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1621a-117">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="1621a-117">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="1621a-118">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="1621a-118">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1621a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1621a-119">Request headers</span></span>
| <span data-ttu-id="1621a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1621a-120">Name</span></span>       | <span data-ttu-id="1621a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1621a-121">Type</span></span> | <span data-ttu-id="1621a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1621a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1621a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1621a-123">Authorization</span></span>  | <span data-ttu-id="1621a-124">string</span><span class="sxs-lookup"><span data-stu-id="1621a-124">string</span></span>  | <span data-ttu-id="1621a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1621a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1621a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1621a-127">Accept</span></span> | <span data-ttu-id="1621a-128">string</span><span class="sxs-lookup"><span data-stu-id="1621a-128">string</span></span> | `application/json` |  

## <a name="request-body"></a><span data-ttu-id="1621a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1621a-129">Request body</span></span>
<span data-ttu-id="1621a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1621a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1621a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1621a-131">Response</span></span>

<span data-ttu-id="1621a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1621a-132">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1621a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1621a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1621a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1621a-134">Request</span></span>
<span data-ttu-id="1621a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1621a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="1621a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1621a-136">Response</span></span>
<span data-ttu-id="1621a-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1621a-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
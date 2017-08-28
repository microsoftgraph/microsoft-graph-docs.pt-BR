# <a name="list-sectiongroups"></a><span data-ttu-id="af200-101">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="af200-101">List sectionGroups</span></span>

<span data-ttu-id="af200-102">Recupere uma lista de objetos[sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="af200-102">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="af200-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="af200-103">Permissions</span></span>
<span data-ttu-id="af200-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af200-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af200-106">Permission type</span></span>      | <span data-ttu-id="af200-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af200-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="af200-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af200-108">Delegated (work or school account)</span></span> | <span data-ttu-id="af200-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af200-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="af200-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af200-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af200-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af200-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="af200-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af200-112">Application</span></span> | <span data-ttu-id="af200-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af200-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="af200-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af200-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af200-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af200-115">Optional query parameters</span></span>
<span data-ttu-id="af200-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af200-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="af200-117">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="af200-117">The default sort order is `name asc`.</span></span>

<span data-ttu-id="af200-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `sections`, `sectionGroups`, `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="af200-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af200-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af200-120">Request headers</span></span>
| <span data-ttu-id="af200-121">Nome</span><span class="sxs-lookup"><span data-stu-id="af200-121">Name</span></span>       | <span data-ttu-id="af200-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="af200-122">Type</span></span> | <span data-ttu-id="af200-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="af200-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af200-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="af200-124">Authorization</span></span>  | <span data-ttu-id="af200-125">string</span><span class="sxs-lookup"><span data-stu-id="af200-125">string</span></span>  | <span data-ttu-id="af200-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af200-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af200-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af200-128">Accept</span></span> | <span data-ttu-id="af200-129">string</span><span class="sxs-lookup"><span data-stu-id="af200-129">string</span></span> | `application/json` |  

## <a name="request-body"></a><span data-ttu-id="af200-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af200-130">Request body</span></span>
<span data-ttu-id="af200-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af200-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af200-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="af200-132">Response</span></span>

<span data-ttu-id="af200-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af200-133">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af200-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af200-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af200-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af200-135">Request</span></span>
<span data-ttu-id="af200-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af200-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="af200-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="af200-137">Response</span></span>
<span data-ttu-id="af200-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af200-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
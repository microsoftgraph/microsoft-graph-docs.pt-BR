# <a name="list-teachers"></a><span data-ttu-id="cc2e0-101">Listar professores</span><span class="sxs-lookup"><span data-stu-id="cc2e0-101">List teachers</span></span>

<span data-ttu-id="cc2e0-102">Recupere uma lista de professores de uma aula.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-102">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="cc2e0-103">Os tokens delegados devem ser membros da aula para obterem a lista de professores.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-103">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc2e0-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc2e0-104">Permissions</span></span>
<span data-ttu-id="cc2e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc2e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc2e0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc2e0-107">Permission type</span></span>      | <span data-ttu-id="cc2e0-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc2e0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc2e0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc2e0-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="cc2e0-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="cc2e0-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="cc2e0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc2e0-111">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="cc2e0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-112">Not supported.</span></span>  |
|<span data-ttu-id="cc2e0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc2e0-113">Application</span></span> | <span data-ttu-id="cc2e0-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc2e0-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cc2e0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc2e0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc2e0-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc2e0-116">Optional query parameters</span></span>
<span data-ttu-id="cc2e0-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc2e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc2e0-118">Request headers</span></span>
| <span data-ttu-id="cc2e0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc2e0-119">Header</span></span>       | <span data-ttu-id="cc2e0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cc2e0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc2e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc2e0-121">Authorization</span></span>  | <span data-ttu-id="cc2e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc2e0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc2e0-124">Request body</span></span>
<span data-ttu-id="cc2e0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cc2e0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc2e0-126">Response</span></span>
<span data-ttu-id="cc2e0-127">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc2e0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc2e0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc2e0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc2e0-129">Request</span></span>
<span data-ttu-id="cc2e0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/11023/teachers
```
##### <a name="response"></a><span data-ttu-id="cc2e0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc2e0-131">Response</span></span>
<span data-ttu-id="cc2e0-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-132">The following is an example of the response.</span></span> 

><span data-ttu-id="cc2e0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc2e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="list-members"></a><span data-ttu-id="b87b2-101">Listar membros</span><span class="sxs-lookup"><span data-stu-id="b87b2-101">List members</span></span>

<span data-ttu-id="b87b2-102">Recupere os professores e alunos de uma aula.</span><span class="sxs-lookup"><span data-stu-id="b87b2-102">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="b87b2-103">Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.</span><span class="sxs-lookup"><span data-stu-id="b87b2-103">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="b87b2-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="b87b2-104">Permissions</span></span>
<span data-ttu-id="b87b2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b87b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b87b2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b87b2-107">Permission type</span></span>      | <span data-ttu-id="b87b2-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b87b2-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b87b2-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b87b2-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="b87b2-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b87b2-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b87b2-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b87b2-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b87b2-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b87b2-112">Not supported</span></span>  |
|<span data-ttu-id="b87b2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b87b2-113">Application</span></span> | <span data-ttu-id="b87b2-114">EduRoster.Read.All, EduRoster.ReadWrite.All mais Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="b87b2-114">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b87b2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b87b2-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b87b2-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b87b2-116">Optional query parameters</span></span>
<span data-ttu-id="b87b2-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b87b2-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b87b2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b87b2-118">Request headers</span></span>
| <span data-ttu-id="b87b2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b87b2-119">Header</span></span>       | <span data-ttu-id="b87b2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b87b2-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b87b2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b87b2-121">Authorization</span></span>  | <span data-ttu-id="b87b2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b87b2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b87b2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b87b2-124">Request body</span></span>
<span data-ttu-id="b87b2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b87b2-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b87b2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b87b2-126">Response</span></span>
<span data-ttu-id="b87b2-127">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b87b2-127">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b87b2-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b87b2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b87b2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b87b2-129">Request</span></span>
<span data-ttu-id="b87b2-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b87b2-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="b87b2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b87b2-131">Response</span></span>
<span data-ttu-id="b87b2-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b87b2-132">The following is an example of the response.</span></span> 

><span data-ttu-id="b87b2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b87b2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

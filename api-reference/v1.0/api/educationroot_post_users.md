# <a name="create-educationuser"></a><span data-ttu-id="c0fb4-101">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="c0fb4-101">Create educationUser</span></span>

<span data-ttu-id="c0fb4-102">Crie um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-102">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="c0fb4-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0fb4-103">Permissions</span></span>
<span data-ttu-id="c0fb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c0fb4-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0fb4-106">Permission type</span></span>      | <span data-ttu-id="c0fb4-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0fb4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0fb4-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0fb4-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0fb4-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-109">Not supported.</span></span>  |
|<span data-ttu-id="c0fb4-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0fb4-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0fb4-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-111">Not supported.</span></span>  |
|<span data-ttu-id="c0fb4-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0fb4-112">Application</span></span> | <span data-ttu-id="c0fb4-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fb4-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c0fb4-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0fb4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="c0fb4-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0fb4-115">Request headers</span></span>
| <span data-ttu-id="c0fb4-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0fb4-116">Header</span></span>       | <span data-ttu-id="c0fb4-117">Valor</span><span class="sxs-lookup"><span data-stu-id="c0fb4-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0fb4-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0fb4-118">Authorization</span></span>  | <span data-ttu-id="c0fb4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0fb4-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0fb4-121">Content-Type</span></span>  | <span data-ttu-id="c0fb4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c0fb4-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0fb4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0fb4-123">Request body</span></span>
<span data-ttu-id="c0fb4-124">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="c0fb4-124">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c0fb4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0fb4-125">Response</span></span>
<span data-ttu-id="c0fb4-126">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-126">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0fb4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0fb4-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0fb4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0fb4-128">Request</span></span>
<span data-ttu-id="c0fb4-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

##### <a name="response"></a><span data-ttu-id="c0fb4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0fb4-130">Response</span></span>
<span data-ttu-id="c0fb4-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-131">The following is an example of the response.</span></span> 

><span data-ttu-id="c0fb4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
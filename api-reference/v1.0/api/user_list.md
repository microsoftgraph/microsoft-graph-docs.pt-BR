# <a name="list-users"></a><span data-ttu-id="defcb-101">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="defcb-101">List users</span></span>

<span data-ttu-id="defcb-102">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="defcb-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="defcb-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="defcb-103">Permissions</span></span>

<span data-ttu-id="defcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="defcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="defcb-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="defcb-106">Permission type</span></span>      | <span data-ttu-id="defcb-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="defcb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="defcb-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="defcb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="defcb-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="defcb-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="defcb-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="defcb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="defcb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="defcb-111">Not supported.</span></span>    |
|<span data-ttu-id="defcb-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="defcb-112">Application</span></span> | <span data-ttu-id="defcb-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="defcb-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="defcb-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="defcb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="defcb-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="defcb-115">Optional query parameters</span></span>

<span data-ttu-id="defcb-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="defcb-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="defcb-117">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="defcb-117">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="defcb-118">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="defcb-118">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="defcb-119">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="defcb-119">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="defcb-p103">Observação: Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário. As seguintes propriedades só terão suporte na [recuperação de um único usuário](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="defcb-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="defcb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="defcb-122">Request headers</span></span>

| <span data-ttu-id="defcb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="defcb-123">Header</span></span>        | <span data-ttu-id="defcb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="defcb-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="defcb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="defcb-125">Authorization</span></span> | <span data-ttu-id="defcb-126">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="defcb-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="defcb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="defcb-127">Content-Type</span></span>  | <span data-ttu-id="defcb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="defcb-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="defcb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="defcb-129">Request body</span></span>

<span data-ttu-id="defcb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="defcb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="defcb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="defcb-131">Response</span></span>

<span data-ttu-id="defcb-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="defcb-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="defcb-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="defcb-133">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="defcb-134">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="defcb-134">Example 1: Standard users request</span></span>

<span data-ttu-id="defcb-135">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="defcb-135">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="defcb-136">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="defcb-136">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="defcb-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="defcb-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="defcb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="defcb-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="defcb-139">Exemplo 2: Solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="defcb-139">Example 2: Users request using $select</span></span>

<span data-ttu-id="defcb-140">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="defcb-140">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="defcb-141">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="defcb-141">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="defcb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="defcb-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="defcb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="defcb-143">Response</span></span>

<span data-ttu-id="defcb-144">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="defcb-144">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

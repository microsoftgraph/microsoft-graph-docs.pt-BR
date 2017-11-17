# <a name="get-a-user"></a><span data-ttu-id="7b4c2-101">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="7b4c2-101">Get a user</span></span>

<span data-ttu-id="7b4c2-102">Recupere as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="7b4c2-p101">Observação: Obter um usuário retorna uma coleção padrão de propriedades somente (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` para obter outras propriedades e relacionamentos para o objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7b4c2-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b4c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b4c2-105">Permissions</span></span>
<span data-ttu-id="7b4c2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b4c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b4c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b4c2-108">Permission type</span></span>      | <span data-ttu-id="7b4c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b4c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b4c2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b4c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b4c2-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b4c2-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b4c2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b4c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b4c2-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b4c2-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="7b4c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b4c2-114">Application</span></span> | <span data-ttu-id="7b4c2-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4c2-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b4c2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b4c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b4c2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b4c2-117">Optional query parameters</span></span>
<span data-ttu-id="7b4c2-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7b4c2-119">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="7b4c2-119">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="7b4c2-120">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return displayName, givenName, id and postalCode, you would use the add the following to your query </span></span> <span data-ttu-id="7b4c2-121">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="7b4c2-121">To return an alternative property set, you must specify the desired set of user properties using the ODATA  query parameter. For example, to return _displayName_, _givenName, id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b4c2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b4c2-122">Request headers</span></span>
| <span data-ttu-id="7b4c2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b4c2-123">Header</span></span>       | <span data-ttu-id="7b4c2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7b4c2-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="7b4c2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b4c2-125">Authorization</span></span>  | <span data-ttu-id="7b4c2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b4c2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b4c2-128">Content-Type</span></span>   | <span data-ttu-id="7b4c2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7b4c2-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b4c2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b4c2-130">Request body</span></span>
<span data-ttu-id="7b4c2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b4c2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b4c2-132">Response</span></span>

<span data-ttu-id="7b4c2-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b4c2-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b4c2-134">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="7b4c2-135">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="7b4c2-135">Example 1: Standard users request</span></span>

<span data-ttu-id="7b4c2-136">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="7b4c2-136">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="7b4c2-137">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-137">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="7b4c2-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b4c2-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="7b4c2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b4c2-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="7b4c2-140">Exemplo 2: Solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="7b4c2-140">Example 2: Users request using $select</span></span>

<span data-ttu-id="7b4c2-141">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-141">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="7b4c2-142">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="7b4c2-142">To return an alternative property set, you must specify the desired set of user properties using the ODATA  query parameter. For example, to return _displayName_, _givenName, id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="7b4c2-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b4c2-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="7b4c2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b4c2-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

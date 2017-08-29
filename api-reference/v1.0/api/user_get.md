# <a name="get-a-user"></a><span data-ttu-id="ceaa7-101">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="ceaa7-101">Get a user</span></span>

<span data-ttu-id="ceaa7-102">Recupere as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="ceaa7-p101">Observação: Obter um usuário retorna uma coleção padrão de propriedades somente (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` para obter outras propriedades e relacionamentos para o objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ceaa7-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceaa7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ceaa7-105">Permissions</span></span>
<span data-ttu-id="ceaa7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ceaa7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ceaa7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceaa7-108">Permission type</span></span>      | <span data-ttu-id="ceaa7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ceaa7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceaa7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceaa7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ceaa7-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ceaa7-111">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ceaa7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceaa7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceaa7-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceaa7-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="ceaa7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceaa7-114">Application</span></span> | <span data-ttu-id="ceaa7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceaa7-115">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceaa7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceaa7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ceaa7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ceaa7-117">Optional query parameters</span></span>
<span data-ttu-id="ceaa7-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ceaa7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceaa7-119">Request headers</span></span>
| <span data-ttu-id="ceaa7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceaa7-120">Header</span></span>       | <span data-ttu-id="ceaa7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ceaa7-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ceaa7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceaa7-122">Authorization</span></span>  | <span data-ttu-id="ceaa7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ceaa7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ceaa7-125">Content-Type</span></span>   | <span data-ttu-id="ceaa7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ceaa7-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceaa7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceaa7-127">Request body</span></span>
<span data-ttu-id="ceaa7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceaa7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceaa7-129">Response</span></span>

<span data-ttu-id="ceaa7-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-130">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ceaa7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceaa7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ceaa7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceaa7-132">Request</span></span>
<span data-ttu-id="ceaa7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="ceaa7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceaa7-134">Response</span></span>
<span data-ttu-id="ceaa7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceaa7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

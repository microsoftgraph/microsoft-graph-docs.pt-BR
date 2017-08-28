# <a name="list-users"></a><span data-ttu-id="91535-101">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="91535-101">List users</span></span>

<span data-ttu-id="91535-102">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="91535-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="91535-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="91535-103">Permissions</span></span>

<span data-ttu-id="91535-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91535-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91535-106">Permission type</span></span>      | <span data-ttu-id="91535-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91535-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="91535-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91535-108">Delegated (work or school account)</span></span> | <span data-ttu-id="91535-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91535-109">One of the following scopes is required to execute this API: User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="91535-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91535-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91535-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91535-111">Not supported.</span></span>    | 
|<span data-ttu-id="91535-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91535-112">Application</span></span> | <span data-ttu-id="91535-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91535-113">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91535-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91535-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91535-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91535-115">Optional query parameters</span></span>

<span data-ttu-id="91535-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91535-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="91535-117">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="91535-117">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="91535-p102">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta ODATA `$select`. Por exemplo, para retornar _displayName_, _givenName_, _id_ e _postalCode_, você pode adicionar o seguinte à sua consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="91535-p102">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return _displayName_, _givenName_, _id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="91535-p103">Observação: Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário. As seguintes propriedades só terão suporte na [recuperação de um único usuário](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="91535-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="91535-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91535-122">Request headers</span></span>

| <span data-ttu-id="91535-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91535-123">Header</span></span>        | <span data-ttu-id="91535-124">Valor</span><span class="sxs-lookup"><span data-stu-id="91535-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="91535-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="91535-125">Authorization</span></span> | <span data-ttu-id="91535-126">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="91535-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="91535-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91535-127">Content-Type</span></span>  | <span data-ttu-id="91535-128">application/json</span><span class="sxs-lookup"><span data-stu-id="91535-128">application/json</span></span>           | 

## <a name="request-body"></a><span data-ttu-id="91535-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91535-129">Request body</span></span>

<span data-ttu-id="91535-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91535-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91535-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="91535-131">Response</span></span>

<span data-ttu-id="91535-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91535-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91535-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91535-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="91535-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91535-134">Request</span></span>

<span data-ttu-id="91535-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91535-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="91535-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="91535-136">Response</span></span>

<span data-ttu-id="91535-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91535-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

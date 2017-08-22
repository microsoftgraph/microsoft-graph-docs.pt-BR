# <a name="create-user"></a><span data-ttu-id="bb5f8-101">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="bb5f8-101">Create User</span></span>

<span data-ttu-id="bb5f8-p101">Use essa API para criar um novo Usuário. O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb5f8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb5f8-106">Prerequisites</span></span>
<span data-ttu-id="bb5f8-107">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="bb5f8-107">One of the following **scopes** is required to execute this API: *User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="bb5f8-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb5f8-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="bb5f8-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5f8-109">Request headers</span></span>
| <span data-ttu-id="bb5f8-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb5f8-110">Header</span></span>       | <span data-ttu-id="bb5f8-111">Valor</span><span class="sxs-lookup"><span data-stu-id="bb5f8-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb5f8-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb5f8-112">Authorization</span></span>  | <span data-ttu-id="bb5f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb5f8-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb5f8-115">Content-Type</span></span>  | <span data-ttu-id="bb5f8-116">application/json</span><span class="sxs-lookup"><span data-stu-id="bb5f8-116">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb5f8-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5f8-117">Request body</span></span>
<span data-ttu-id="bb5f8-118">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bb5f8-118">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="bb5f8-119">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-119">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="bb5f8-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bb5f8-120">Parameter</span></span> | <span data-ttu-id="bb5f8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb5f8-121">Type</span></span> | <span data-ttu-id="bb5f8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb5f8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb5f8-123">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="bb5f8-123">accountEnabled</span></span> |<span data-ttu-id="bb5f8-124">booliano</span><span class="sxs-lookup"><span data-stu-id="bb5f8-124">boolean</span></span> |<span data-ttu-id="bb5f8-125">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-125">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="bb5f8-126">displayName</span><span class="sxs-lookup"><span data-stu-id="bb5f8-126">displayName</span></span> |<span data-ttu-id="bb5f8-127">string</span><span class="sxs-lookup"><span data-stu-id="bb5f8-127">string</span></span> |<span data-ttu-id="bb5f8-128">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-128">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="bb5f8-129">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="bb5f8-129">onPremisesImmutableId</span></span> |<span data-ttu-id="bb5f8-130">string</span><span class="sxs-lookup"><span data-stu-id="bb5f8-130">string</span></span> |<span data-ttu-id="bb5f8-131">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-131">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="bb5f8-132">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bb5f8-132">mailNickname</span></span> |<span data-ttu-id="bb5f8-133">string</span><span class="sxs-lookup"><span data-stu-id="bb5f8-133">string</span></span> |<span data-ttu-id="bb5f8-134">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-134">The mail alias for the user.</span></span>|
|<span data-ttu-id="bb5f8-135">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="bb5f8-135">passwordProfile</span></span>|[<span data-ttu-id="bb5f8-136">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="bb5f8-136">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="bb5f8-137">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-137">The password profile for the user.</span></span>|
|<span data-ttu-id="bb5f8-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb5f8-138">userPrincipalName</span></span> |<span data-ttu-id="bb5f8-139">string</span><span class="sxs-lookup"><span data-stu-id="bb5f8-139">string</span></span> |<span data-ttu-id="bb5f8-140">Nome UPN (someuser@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="bb5f8-140">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="bb5f8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5f8-141">Response</span></span>

<span data-ttu-id="bb5f8-142">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-142">If successful, this method returns `201, Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb5f8-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb5f8-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb5f8-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5f8-144">Request</span></span>
<span data-ttu-id="bb5f8-145">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="bb5f8-146">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bb5f8-146">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bb5f8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5f8-147">Response</span></span>
<span data-ttu-id="bb5f8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb5f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

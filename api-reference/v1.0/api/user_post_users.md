# <a name="create-user"></a><span data-ttu-id="c6c4b-101">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="c6c4b-101">Create User</span></span>

<span data-ttu-id="c6c4b-p101">Use essa API para criar um novo Usuário. O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6c4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6c4b-106">Permissions</span></span>
<span data-ttu-id="c6c4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6c4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c6c4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6c4b-109">Permission type</span></span>      | <span data-ttu-id="c6c4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6c4b-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c6c4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6c4b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6c4b-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6c4b-112">One of the following scopes is required to execute this API: User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="c6c4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6c4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6c4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-114">Not supported.</span></span>    | 
|<span data-ttu-id="c6c4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6c4b-115">Application</span></span> | <span data-ttu-id="c6c4b-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c4b-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c6c4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6c4b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="c6c4b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c4b-118">Request headers</span></span>
| <span data-ttu-id="c6c4b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6c4b-119">Header</span></span>       | <span data-ttu-id="c6c4b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c6c4b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6c4b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6c4b-121">Authorization</span></span>  | <span data-ttu-id="c6c4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6c4b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6c4b-124">Content-Type</span></span>  | <span data-ttu-id="c6c4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6c4b-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6c4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c4b-126">Request body</span></span>
<span data-ttu-id="c6c4b-127">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c6c4b-127">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="c6c4b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="c6c4b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c6c4b-129">Parameter</span></span> | <span data-ttu-id="c6c4b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6c4b-130">Type</span></span> | <span data-ttu-id="c6c4b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6c4b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6c4b-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="c6c4b-132">accountEnabled</span></span> |<span data-ttu-id="c6c4b-133">booliano</span><span class="sxs-lookup"><span data-stu-id="c6c4b-133">boolean</span></span> |<span data-ttu-id="c6c4b-134">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-134">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="c6c4b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c6c4b-135">displayName</span></span> |<span data-ttu-id="c6c4b-136">string</span><span class="sxs-lookup"><span data-stu-id="c6c4b-136">string</span></span> |<span data-ttu-id="c6c4b-137">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-137">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="c6c4b-138">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="c6c4b-138">onPremisesImmutableId</span></span> |<span data-ttu-id="c6c4b-139">string</span><span class="sxs-lookup"><span data-stu-id="c6c4b-139">string</span></span> |<span data-ttu-id="c6c4b-140">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-140">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="c6c4b-141">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c6c4b-141">mailNickname</span></span> |<span data-ttu-id="c6c4b-142">string</span><span class="sxs-lookup"><span data-stu-id="c6c4b-142">string</span></span> |<span data-ttu-id="c6c4b-143">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-143">The mail alias for the user.</span></span>|
|<span data-ttu-id="c6c4b-144">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="c6c4b-144">passwordProfile</span></span>|[<span data-ttu-id="c6c4b-145">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="c6c4b-145">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="c6c4b-146">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-146">The password profile for the user.</span></span>|
|<span data-ttu-id="c6c4b-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6c4b-147">userPrincipalName</span></span> |<span data-ttu-id="c6c4b-148">string</span><span class="sxs-lookup"><span data-stu-id="c6c4b-148">string</span></span> |<span data-ttu-id="c6c4b-149">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c6c4b-149">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="c6c4b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c4b-150">Response</span></span>

<span data-ttu-id="c6c4b-151">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-151">If successful, this method returns `201, Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6c4b-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6c4b-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6c4b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c4b-153">Request</span></span>
<span data-ttu-id="c6c4b-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-154">Here is an example of the request.</span></span>
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
<span data-ttu-id="c6c4b-155">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c6c4b-155">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c6c4b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c4b-156">Response</span></span>
<span data-ttu-id="c6c4b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6c4b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

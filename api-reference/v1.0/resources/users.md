# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="85a32-101">Trabalhando com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="85a32-101">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="85a32-102">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="85a32-102">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="85a32-103">Você pode acessar [usuários](user.md) pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="85a32-103">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="85a32-104">Por sua ID, `/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="85a32-104">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="85a32-105">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="85a32-105">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="85a32-106">Autorização</span><span class="sxs-lookup"><span data-stu-id="85a32-106">Authorization</span></span>

<span data-ttu-id="85a32-p101">Uma das seguintes [permissões](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="85a32-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="85a32-110">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="85a32-110">User.ReadBasic.All</span></span>
- <span data-ttu-id="85a32-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="85a32-111">User.Read</span></span>
- <span data-ttu-id="85a32-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85a32-112">User.ReadWrite</span></span>
- <span data-ttu-id="85a32-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85a32-113">User.Read.All</span></span>
- <span data-ttu-id="85a32-114">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85a32-114">User.ReadWrite.All</span></span>
- <span data-ttu-id="85a32-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="85a32-115">Directory.Read.All</span></span>
- <span data-ttu-id="85a32-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85a32-116">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="85a32-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85a32-117">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="85a32-118">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="85a32-118">Common properties</span></span>

<span data-ttu-id="85a32-119">O item a seguir representa o conjunto padrão de propriedades que serão retornadas ao se obter um usuário ou listar usuários.</span><span class="sxs-lookup"><span data-stu-id="85a32-119">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="85a32-120">Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="85a32-120">These are a subset of all available properties.</span></span> <span data-ttu-id="85a32-121">Para obter mais propriedades do usuário, use o parâmetro de consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="85a32-121">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="85a32-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85a32-122">Property</span></span> |<span data-ttu-id="85a32-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="85a32-123">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="85a32-124">id</span><span class="sxs-lookup"><span data-stu-id="85a32-124">id</span></span> | <span data-ttu-id="85a32-125">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-125">The unique identifier for the user.</span></span>|
|<span data-ttu-id="85a32-126">businessPhones</span><span class="sxs-lookup"><span data-stu-id="85a32-126">businessPhones</span></span> | <span data-ttu-id="85a32-127">Os números de telefone do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-127">The user's phone numbers.</span></span>|
|<span data-ttu-id="85a32-128">displayName</span><span class="sxs-lookup"><span data-stu-id="85a32-128">displayName</span></span> | <span data-ttu-id="85a32-129">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-129">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="85a32-130">givenName</span><span class="sxs-lookup"><span data-stu-id="85a32-130">givenName</span></span>| <span data-ttu-id="85a32-131">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-131">The first name of the user.</span></span> |
|<span data-ttu-id="85a32-132">jobTitle</span><span class="sxs-lookup"><span data-stu-id="85a32-132">jobTitle</span></span> | <span data-ttu-id="85a32-133">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-133">The user's job title.</span></span>|
|<span data-ttu-id="85a32-134">email</span><span class="sxs-lookup"><span data-stu-id="85a32-134">mail</span></span>| <span data-ttu-id="85a32-135">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-135">The user's email address.</span></span> |
|<span data-ttu-id="85a32-136">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="85a32-136">mobilePhone</span></span> | <span data-ttu-id="85a32-137">O número de telefone celular do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-137">The user's cellphone number.</span></span>|
|<span data-ttu-id="85a32-138">officeLocation</span><span class="sxs-lookup"><span data-stu-id="85a32-138">officeLocation</span></span> | <span data-ttu-id="85a32-139">O local do escritório físico do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-139">The user's physical office location.</span></span>|
|<span data-ttu-id="85a32-140">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="85a32-140">preferredLanguage</span></span> | <span data-ttu-id="85a32-141">O idioma preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-141">The user's language of preference.</span></span>|
|<span data-ttu-id="85a32-142">surname</span><span class="sxs-lookup"><span data-stu-id="85a32-142">surname</span></span>| <span data-ttu-id="85a32-143">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-143">The last name of the user.</span></span> |
|<span data-ttu-id="85a32-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85a32-144">userPrincipalName</span></span>| <span data-ttu-id="85a32-145">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-145">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="85a32-146">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="85a32-146">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="85a32-147">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="85a32-147">Common operations</span></span>

> <span data-ttu-id="85a32-148">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="85a32-148">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="85a32-149">Path</span><span class="sxs-lookup"><span data-stu-id="85a32-149">Path</span></span>    | <span data-ttu-id="85a32-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="85a32-150">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user_list.md) | <span data-ttu-id="85a32-151">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="85a32-151">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user_get.md) | <span data-ttu-id="85a32-152">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="85a32-152">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto_get.md)| <span data-ttu-id="85a32-153">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-153">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user_list_manager.md) | <span data-ttu-id="85a32-154">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-154">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user_list_messages.md)| <span data-ttu-id="85a32-155">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="85a32-155">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user_list_events.md) | <span data-ttu-id="85a32-156">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="85a32-156">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive_get.md)| <span data-ttu-id="85a32-157">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="85a32-157">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user_list_memberof.md)| <span data-ttu-id="85a32-158">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="85a32-158">Lists the groups that the user is a member of.</span></span> |

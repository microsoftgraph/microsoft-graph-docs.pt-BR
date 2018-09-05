# <a name="create-group"></a><span data-ttu-id="88048-101">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="88048-101">Create group</span></span>
<span data-ttu-id="88048-p101">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="88048-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="88048-104">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="88048-104">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="88048-105">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="88048-105">Dynamic group</span></span>
* <span data-ttu-id="88048-106">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="88048-106">Security group</span></span>

> <span data-ttu-id="88048-p102">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="88048-p102">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="88048-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="88048-109">Permissions</span></span>
<span data-ttu-id="88048-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88048-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88048-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88048-112">Permission type</span></span>      | <span data-ttu-id="88048-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88048-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88048-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88048-114">Delegated (work or school account)</span></span> | <span data-ttu-id="88048-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88048-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="88048-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88048-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88048-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88048-117">Not supported.</span></span>    |
|<span data-ttu-id="88048-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88048-118">Application</span></span> | <span data-ttu-id="88048-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88048-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88048-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88048-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="88048-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88048-121">Request headers</span></span>
| <span data-ttu-id="88048-122">Nome</span><span class="sxs-lookup"><span data-stu-id="88048-122">Name</span></span>       | <span data-ttu-id="88048-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="88048-123">Type</span></span> | <span data-ttu-id="88048-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="88048-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88048-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="88048-125">Authorization</span></span>  | <span data-ttu-id="88048-126">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88048-126">string</span></span>  | <span data-ttu-id="88048-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88048-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88048-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88048-129">Request body</span></span>
<span data-ttu-id="88048-130">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar ao criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="88048-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="88048-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88048-131">Property</span></span> | <span data-ttu-id="88048-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="88048-132">Type</span></span> | <span data-ttu-id="88048-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="88048-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88048-134">displayName</span><span class="sxs-lookup"><span data-stu-id="88048-134">displayName</span></span> | <span data-ttu-id="88048-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88048-135">string</span></span> | <span data-ttu-id="88048-136">O nome de exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="88048-136">The name to display in the address book for the group.</span></span> <span data-ttu-id="88048-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88048-137">Required.</span></span> |
| <span data-ttu-id="88048-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="88048-138">mailEnabled</span></span> | <span data-ttu-id="88048-139">booleano</span><span class="sxs-lookup"><span data-stu-id="88048-139">boolean</span></span> | <span data-ttu-id="88048-140">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="88048-140">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="88048-141">Defina como **true** se estiver criando um grupo no Office 365.</span><span class="sxs-lookup"><span data-stu-id="88048-141">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="88048-142">Defina como **false** se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="88048-142">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="88048-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88048-143">Required.</span></span> |
| <span data-ttu-id="88048-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="88048-144">mailNickname</span></span> | <span data-ttu-id="88048-145">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88048-145">string</span></span> | <span data-ttu-id="88048-146">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="88048-146">The mail alias for the group.</span></span> <span data-ttu-id="88048-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88048-147">Required.</span></span> |
| <span data-ttu-id="88048-148">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="88048-148">securityEnabled</span></span> | <span data-ttu-id="88048-149">booleano</span><span class="sxs-lookup"><span data-stu-id="88048-149">boolean</span></span> | <span data-ttu-id="88048-150">Defina como **true** para grupos habilitados para segurança.</span><span class="sxs-lookup"><span data-stu-id="88048-150">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="88048-151">Defina como **true** se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="88048-151">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="88048-152">Defina como **false** se estiver criando um grupo no Office 365.</span><span class="sxs-lookup"><span data-stu-id="88048-152">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="88048-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88048-153">Required.</span></span> |
| <span data-ttu-id="88048-154">owners</span><span class="sxs-lookup"><span data-stu-id="88048-154">owners</span></span> | <span data-ttu-id="88048-155">coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88048-155">string collection</span></span> | <span data-ttu-id="88048-156">Essa propriedade representa os proprietários do grupo no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="88048-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="88048-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="88048-157">Optional.</span></span> |
| <span data-ttu-id="88048-158">members</span><span class="sxs-lookup"><span data-stu-id="88048-158">members</span></span> | <span data-ttu-id="88048-159">coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88048-159">string collection</span></span> | <span data-ttu-id="88048-160">Essa propriedade representa os membros do grupo no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="88048-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="88048-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="88048-161">Optional.</span></span> |


<span data-ttu-id="88048-162">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="88048-162">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="88048-163">opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="88048-163">groupTypes options</span></span>

| <span data-ttu-id="88048-164">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="88048-164">Type of group</span></span> | <span data-ttu-id="88048-165">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="88048-165">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="88048-166">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="88048-166">Office 365 (aka unified group)</span></span>| <span data-ttu-id="88048-167">"Unified"</span><span class="sxs-lookup"><span data-stu-id="88048-167">"Unified"</span></span> |
| <span data-ttu-id="88048-168">Dinâmico</span><span class="sxs-lookup"><span data-stu-id="88048-168">Dynamic</span></span> | <span data-ttu-id="88048-169">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="88048-169">"DynamicMembership"</span></span> |
| <span data-ttu-id="88048-170">Segurança</span><span class="sxs-lookup"><span data-stu-id="88048-170">Security</span></span> | <span data-ttu-id="88048-171">Não defina.</span><span class="sxs-lookup"><span data-stu-id="88048-171">Do not set.</span></span> |


><span data-ttu-id="88048-172">**Observação:** Criar um grupo do Office 365 via programação sem um contexto de usuário e sem a especificação de proprietários criará o grupo de forma anônima.</span><span class="sxs-lookup"><span data-stu-id="88048-172">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="88048-173">Dessa forma, o site associado do SharePoint Online poderá não ser criado automaticamente até que uma ação manual seja realizada.</span><span class="sxs-lookup"><span data-stu-id="88048-173">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="88048-p112">Especifique outras propriedades graváveis para o seu grupo conforme necessário. Para obter mais informações, confira as propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="88048-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="88048-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="88048-176">Response</span></span>
<span data-ttu-id="88048-177">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88048-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88048-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88048-178">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="88048-179">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="88048-179">Request 1</span></span>
<span data-ttu-id="88048-180">O primeiro exemplo de solicitação cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="88048-180">The following is an example of a request that creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a><span data-ttu-id="88048-181">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="88048-181">Response 1</span></span>
<span data-ttu-id="88048-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88048-182">The following is an example of the response.</span></span>
><span data-ttu-id="88048-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para melhor legibilidade. Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88048-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a><span data-ttu-id="88048-185">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="88048-185">Request 2</span></span>
<span data-ttu-id="88048-186">O segundo exemplo de solicitação cria um grupo do Office 365 com proprietários especificados.</span><span class="sxs-lookup"><span data-stu-id="88048-186">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="88048-187">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="88048-187">Response 2</span></span>
<span data-ttu-id="88048-188">Este é um exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="88048-188">The following is an example of the response.</span></span>
><span data-ttu-id="88048-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para melhor legibilidade. Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88048-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

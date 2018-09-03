# <a name="create-group"></a><span data-ttu-id="cf6f1-101">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="cf6f1-101">Create group</span></span>
<span data-ttu-id="cf6f1-p101">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="cf6f1-104">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="cf6f1-104">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="cf6f1-105">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="cf6f1-105">Dynamic group</span></span>
* <span data-ttu-id="cf6f1-106">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="cf6f1-106">Security group</span></span>

> <span data-ttu-id="cf6f1-p102">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p102">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf6f1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf6f1-109">Permissions</span></span>
<span data-ttu-id="cf6f1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf6f1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf6f1-112">Permission type</span></span>      | <span data-ttu-id="cf6f1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf6f1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf6f1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf6f1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cf6f1-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf6f1-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf6f1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf6f1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf6f1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-117">Not supported.</span></span>    |
|<span data-ttu-id="cf6f1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf6f1-118">Application</span></span> | <span data-ttu-id="cf6f1-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf6f1-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf6f1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf6f1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="cf6f1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf6f1-121">Request headers</span></span>
| <span data-ttu-id="cf6f1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cf6f1-122">Name</span></span>       | <span data-ttu-id="cf6f1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf6f1-123">Type</span></span> | <span data-ttu-id="cf6f1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf6f1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf6f1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf6f1-125">Authorization</span></span>  | <span data-ttu-id="cf6f1-126">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6f1-126">string</span></span>  | <span data-ttu-id="cf6f1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf6f1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf6f1-129">Request body</span></span>
<span data-ttu-id="cf6f1-130">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar no mínimo quando cria um grupo.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="cf6f1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf6f1-131">Property</span></span> | <span data-ttu-id="cf6f1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf6f1-132">Type</span></span> | <span data-ttu-id="cf6f1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf6f1-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf6f1-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cf6f1-134">displayName</span></span> | <span data-ttu-id="cf6f1-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6f1-135">string</span></span> | <span data-ttu-id="cf6f1-136">O nome de exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-136">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="cf6f1-137">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="cf6f1-137">mailEnabled</span></span> | <span data-ttu-id="cf6f1-138">booliano</span><span class="sxs-lookup"><span data-stu-id="cf6f1-138">boolean</span></span> | <span data-ttu-id="cf6f1-p105">Defina como **true** para grupos habilitados para email. Defina como **true** se estiver criando um grupo do Office 365. Defina como **false** se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p105">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 Group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="cf6f1-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cf6f1-142">mailNickname</span></span> | <span data-ttu-id="cf6f1-143">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6f1-143">string</span></span> | <span data-ttu-id="cf6f1-144">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-144">The mail alias for the group.</span></span> |
| <span data-ttu-id="cf6f1-145">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="cf6f1-145">securityEnabled</span></span> | <span data-ttu-id="cf6f1-146">booliano</span><span class="sxs-lookup"><span data-stu-id="cf6f1-146">boolean</span></span> | <span data-ttu-id="cf6f1-p106">Defina como **true** para grupos de segurança. Definir isto como **true** se estiver criando um grupo dinâmico ou de segurança. Defina isto como **false** se estiver criando um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p106">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="cf6f1-150">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-150">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="cf6f1-151">opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="cf6f1-151">groupTypes options</span></span>

| <span data-ttu-id="cf6f1-152">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="cf6f1-152">Type of group</span></span> | <span data-ttu-id="cf6f1-153">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="cf6f1-153">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="cf6f1-154">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="cf6f1-154">Office 365 (aka unified group)</span></span>| <span data-ttu-id="cf6f1-155">"Unified"</span><span class="sxs-lookup"><span data-stu-id="cf6f1-155">"Unified"</span></span> |
| <span data-ttu-id="cf6f1-156">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="cf6f1-156">Dynamic</span></span> | <span data-ttu-id="cf6f1-157">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="cf6f1-157">"DynamicMembership"</span></span> |
| <span data-ttu-id="cf6f1-158">Segurança</span><span class="sxs-lookup"><span data-stu-id="cf6f1-158">Security</span></span> | <span data-ttu-id="cf6f1-159">Não defina.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-159">Do not set.</span></span> |

<span data-ttu-id="cf6f1-p107">Especifique outras propriedades graváveis conforme necessário para o seu grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p107">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="cf6f1-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf6f1-162">Response</span></span>
<span data-ttu-id="cf6f1-163">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-163">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf6f1-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf6f1-164">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cf6f1-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf6f1-165">Request</span></span>
<span data-ttu-id="cf6f1-166">Este é um exemplo de uma solicitação que cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-166">The following is an example of a request that creates an Office 365 Group.</span></span>
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

#### <a name="response"></a><span data-ttu-id="cf6f1-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf6f1-167">Response</span></span>
<span data-ttu-id="cf6f1-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-168">The following is an example of the response.</span></span>
><span data-ttu-id="cf6f1-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf6f1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

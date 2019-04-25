---
title: Criar grupo
description: 'Use esta API para criar um novo grupo, conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 87494b309dd731c519f0d999396f283c5a2fa583
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502125"
---
# <a name="create-group"></a><span data-ttu-id="eb291-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="eb291-104">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb291-p102">Use esta API para criar um novo [grupo](../resources/group.md), conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="eb291-p102">Use this API to create a new [group](../resources/group.md) as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="eb291-107">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="eb291-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="eb291-108">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="eb291-108">Dynamic group</span></span>
* <span data-ttu-id="eb291-109">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="eb291-109">Security group</span></span>

<span data-ttu-id="eb291-110">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="eb291-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="eb291-111">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="eb291-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="eb291-112">Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="eb291-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="eb291-113">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="eb291-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="eb291-114">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="eb291-114">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb291-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb291-115">Permissions</span></span>
<span data-ttu-id="eb291-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb291-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb291-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb291-118">Permission type</span></span>      | <span data-ttu-id="eb291-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb291-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb291-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb291-120">Delegated (work or school account)</span></span> | <span data-ttu-id="eb291-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb291-121">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb291-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb291-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb291-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb291-123">Not supported.</span></span>    |
|<span data-ttu-id="eb291-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb291-124">Application</span></span> | <span data-ttu-id="eb291-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb291-125">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb291-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb291-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="eb291-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb291-127">Request headers</span></span>
| <span data-ttu-id="eb291-128">Nome</span><span class="sxs-lookup"><span data-stu-id="eb291-128">Name</span></span>       | <span data-ttu-id="eb291-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb291-129">Type</span></span> | <span data-ttu-id="eb291-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb291-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb291-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb291-131">Authorization</span></span>  | <span data-ttu-id="eb291-132">string</span><span class="sxs-lookup"><span data-stu-id="eb291-132">string</span></span>  | <span data-ttu-id="eb291-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb291-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb291-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb291-135">Request body</span></span>
<span data-ttu-id="eb291-136">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="eb291-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="eb291-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb291-137">Property</span></span> | <span data-ttu-id="eb291-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb291-138">Type</span></span> | <span data-ttu-id="eb291-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb291-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb291-140">displayName</span><span class="sxs-lookup"><span data-stu-id="eb291-140">displayName</span></span> | <span data-ttu-id="eb291-141">string</span><span class="sxs-lookup"><span data-stu-id="eb291-141">string</span></span> | <span data-ttu-id="eb291-142">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="eb291-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="eb291-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb291-143">Required.</span></span> |
| <span data-ttu-id="eb291-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="eb291-144">mailEnabled</span></span> | <span data-ttu-id="eb291-145">booliano</span><span class="sxs-lookup"><span data-stu-id="eb291-145">boolean</span></span> | <span data-ttu-id="eb291-146">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="eb291-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="eb291-147">Defina isto como **true**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb291-147">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="eb291-148">Defina como **false**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="eb291-148">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="eb291-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb291-149">Required.</span></span> |
| <span data-ttu-id="eb291-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="eb291-150">mailNickname</span></span> | <span data-ttu-id="eb291-151">string</span><span class="sxs-lookup"><span data-stu-id="eb291-151">string</span></span> | <span data-ttu-id="eb291-152">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="eb291-152">The mail alias for the group.</span></span> <span data-ttu-id="eb291-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb291-153">Required.</span></span> |
| <span data-ttu-id="eb291-154">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="eb291-154">securityEnabled</span></span> | <span data-ttu-id="eb291-155">booliano</span><span class="sxs-lookup"><span data-stu-id="eb291-155">boolean</span></span> | <span data-ttu-id="eb291-156">Defina como **true** para grupos habilitados para segurança.</span><span class="sxs-lookup"><span data-stu-id="eb291-156">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="eb291-157">Defina isto como **true**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="eb291-157">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="eb291-158">Defina isto como **false**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb291-158">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="eb291-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb291-159">Required.</span></span> |
| <span data-ttu-id="eb291-160">owners</span><span class="sxs-lookup"><span data-stu-id="eb291-160">owners</span></span> | <span data-ttu-id="eb291-161">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb291-161">string collection</span></span> | <span data-ttu-id="eb291-162">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="eb291-162">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="eb291-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb291-163">Optional.</span></span> |
| <span data-ttu-id="eb291-164">membros</span><span class="sxs-lookup"><span data-stu-id="eb291-164">members</span></span> | <span data-ttu-id="eb291-165">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb291-165">string collection</span></span> | <span data-ttu-id="eb291-166">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="eb291-166">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="eb291-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb291-167">Optional.</span></span> |

<span data-ttu-id="eb291-168">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="eb291-168">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="eb291-169">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="eb291-169">Type of group</span></span> | <span data-ttu-id="eb291-170">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="eb291-170">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="eb291-171">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="eb291-171">Office 365 (aka unified group)</span></span>| <span data-ttu-id="eb291-172">"Unified"</span><span class="sxs-lookup"><span data-stu-id="eb291-172">"Unified"</span></span> |
| <span data-ttu-id="eb291-173">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="eb291-173">Dynamic</span></span> | <span data-ttu-id="eb291-174">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="eb291-174">"DynamicMembership"</span></span> |
| <span data-ttu-id="eb291-175">Segurança</span><span class="sxs-lookup"><span data-stu-id="eb291-175">Security</span></span> | <span data-ttu-id="eb291-176">Não defina.</span><span class="sxs-lookup"><span data-stu-id="eb291-176">Do not set.</span></span> |

<span data-ttu-id="eb291-177">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="eb291-177">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="eb291-178">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="eb291-178">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="eb291-179">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="eb291-179">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="eb291-p114">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="eb291-p114">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="eb291-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb291-182">Response</span></span>
<span data-ttu-id="eb291-183">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb291-183">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="eb291-184">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="eb291-184">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="eb291-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb291-185">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="eb291-186">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="eb291-186">Request 1</span></span>
<span data-ttu-id="eb291-187">A primeira solicitação de exemplo cria um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb291-187">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="eb291-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb291-188">Response</span></span>
<span data-ttu-id="eb291-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb291-189">The following is an example of the response.</span></span>
><span data-ttu-id="eb291-190">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb291-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb291-191">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb291-191">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="eb291-192">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="eb291-192">Request 2</span></span>
<span data-ttu-id="eb291-193">A segunda solicitação de exemplo cria um Grupo do Office 365 com um proprietário especificado.</span><span class="sxs-lookup"><span data-stu-id="eb291-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="eb291-194">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="eb291-194">Response 2</span></span>
<span data-ttu-id="eb291-195">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="eb291-195">The following is an example of a successful response.</span></span> <span data-ttu-id="eb291-196">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="eb291-196">It includes only default properties.</span></span> <span data-ttu-id="eb291-197">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="eb291-197">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="eb291-198">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb291-198">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb291-199">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb291-199">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="eb291-200">Confira também</span><span class="sxs-lookup"><span data-stu-id="eb291-200">See also</span></span>

- [<span data-ttu-id="eb291-201">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="eb291-201">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eb291-202">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="eb291-202">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="eb291-203">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="eb291-203">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

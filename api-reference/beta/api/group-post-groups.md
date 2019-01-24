---
title: Criar grupo
description: 'Use esta API para criar um novo grupo, conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 736c4350cc5c7c57d0b57562676317317f6f74dc
ms.sourcegitcommit: 71368f59d267c8188567529e74486e54cc122804
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29442322"
---
# <a name="create-group"></a><span data-ttu-id="7275f-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="7275f-104">Create group</span></span>

> <span data-ttu-id="7275f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7275f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7275f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7275f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7275f-p103">Use esta API para criar um novo [grupo](../resources/group.md), conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="7275f-p103">Use this API to create a new [group](../resources/group.md) as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="7275f-109">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="7275f-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="7275f-110">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="7275f-110">Dynamic group</span></span>
* <span data-ttu-id="7275f-111">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="7275f-111">Security group</span></span>

<span data-ttu-id="7275f-112">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="7275f-112">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="7275f-113">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="7275f-113">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="7275f-114">Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="7275f-114">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="7275f-115">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="7275f-115">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="7275f-116">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="7275f-116">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7275f-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="7275f-117">Permissions</span></span>
<span data-ttu-id="7275f-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7275f-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7275f-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7275f-120">Permission type</span></span>      | <span data-ttu-id="7275f-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7275f-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7275f-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7275f-122">Delegated (work or school account)</span></span> | <span data-ttu-id="7275f-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7275f-123">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7275f-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7275f-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7275f-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7275f-125">Not supported.</span></span>    |
|<span data-ttu-id="7275f-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7275f-126">Application</span></span> | <span data-ttu-id="7275f-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7275f-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7275f-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7275f-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7275f-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7275f-129">Request headers</span></span>
| <span data-ttu-id="7275f-130">Nome</span><span class="sxs-lookup"><span data-stu-id="7275f-130">Name</span></span>       | <span data-ttu-id="7275f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7275f-131">Type</span></span> | <span data-ttu-id="7275f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7275f-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7275f-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="7275f-133">Authorization</span></span>  | <span data-ttu-id="7275f-134">string</span><span class="sxs-lookup"><span data-stu-id="7275f-134">string</span></span>  | <span data-ttu-id="7275f-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7275f-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7275f-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7275f-137">Request body</span></span>
<span data-ttu-id="7275f-138">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="7275f-138">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7275f-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7275f-139">Property</span></span> | <span data-ttu-id="7275f-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="7275f-140">Type</span></span> | <span data-ttu-id="7275f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="7275f-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7275f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7275f-142">displayName</span></span> | <span data-ttu-id="7275f-143">string</span><span class="sxs-lookup"><span data-stu-id="7275f-143">string</span></span> | <span data-ttu-id="7275f-144">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="7275f-144">The name to display in the address book for the group.</span></span> <span data-ttu-id="7275f-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7275f-145">Required.</span></span> |
| <span data-ttu-id="7275f-146">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7275f-146">mailEnabled</span></span> | <span data-ttu-id="7275f-147">booliano</span><span class="sxs-lookup"><span data-stu-id="7275f-147">boolean</span></span> | <span data-ttu-id="7275f-148">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="7275f-148">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="7275f-149">Defina isto como **true**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7275f-149">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="7275f-150">Defina como **false**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="7275f-150">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="7275f-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7275f-151">Required.</span></span> |
| <span data-ttu-id="7275f-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7275f-152">mailNickname</span></span> | <span data-ttu-id="7275f-153">string</span><span class="sxs-lookup"><span data-stu-id="7275f-153">string</span></span> | <span data-ttu-id="7275f-154">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="7275f-154">The mail alias for the group.</span></span> <span data-ttu-id="7275f-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7275f-155">Required.</span></span> |
| <span data-ttu-id="7275f-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7275f-156">securityEnabled</span></span> | <span data-ttu-id="7275f-157">booliano</span><span class="sxs-lookup"><span data-stu-id="7275f-157">boolean</span></span> | <span data-ttu-id="7275f-158">Defina como **true** para grupos habilitados para segurança.</span><span class="sxs-lookup"><span data-stu-id="7275f-158">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="7275f-159">Defina isto como **true**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="7275f-159">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="7275f-160">Defina isto como **false**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7275f-160">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="7275f-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7275f-161">Required.</span></span> |
| <span data-ttu-id="7275f-162">owners</span><span class="sxs-lookup"><span data-stu-id="7275f-162">owners</span></span> | <span data-ttu-id="7275f-163">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7275f-163">string collection</span></span> | <span data-ttu-id="7275f-164">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="7275f-164">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="7275f-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7275f-165">Optional.</span></span> |
| <span data-ttu-id="7275f-166">membros</span><span class="sxs-lookup"><span data-stu-id="7275f-166">members</span></span> | <span data-ttu-id="7275f-167">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7275f-167">string collection</span></span> | <span data-ttu-id="7275f-168">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="7275f-168">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="7275f-169">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7275f-169">Optional.</span></span> |

<span data-ttu-id="7275f-170">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="7275f-170">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="7275f-171">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="7275f-171">Type of group</span></span> | <span data-ttu-id="7275f-172">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="7275f-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="7275f-173">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="7275f-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="7275f-174">"Unified"</span><span class="sxs-lookup"><span data-stu-id="7275f-174">"Unified"</span></span> |
| <span data-ttu-id="7275f-175">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="7275f-175">Dynamic</span></span> | <span data-ttu-id="7275f-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="7275f-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="7275f-177">Segurança</span><span class="sxs-lookup"><span data-stu-id="7275f-177">Security</span></span> | <span data-ttu-id="7275f-178">Não defina.</span><span class="sxs-lookup"><span data-stu-id="7275f-178">Do not set.</span></span> |

<span data-ttu-id="7275f-179">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="7275f-179">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7275f-180">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="7275f-180">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="7275f-181">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="7275f-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7275f-p115">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7275f-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7275f-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="7275f-184">Response</span></span>
<span data-ttu-id="7275f-185">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7275f-185">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="7275f-186">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="7275f-186">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="7275f-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7275f-187">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="7275f-188">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="7275f-188">Request 1</span></span>
<span data-ttu-id="7275f-189">A primeira solicitação de exemplo cria um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7275f-189">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response"></a><span data-ttu-id="7275f-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="7275f-190">Response</span></span>
<span data-ttu-id="7275f-191">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7275f-191">The following is an example of the response.</span></span>
><span data-ttu-id="7275f-192">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7275f-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7275f-193">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7275f-193">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="7275f-194">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="7275f-194">Request 2</span></span>
<span data-ttu-id="7275f-195">A segunda solicitação de exemplo cria um Grupo do Office 365 com um proprietário especificado.</span><span class="sxs-lookup"><span data-stu-id="7275f-195">The second example request creates an Office 365 group with an owner specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="7275f-196">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="7275f-196">Response 2</span></span>
<span data-ttu-id="7275f-197">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="7275f-197">The following is an example of a successful response.</span></span> <span data-ttu-id="7275f-198">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="7275f-198">It includes only default properties.</span></span> <span data-ttu-id="7275f-199">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="7275f-199">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="7275f-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7275f-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7275f-201">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7275f-201">All the default properties are returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7275f-202">Confira também</span><span class="sxs-lookup"><span data-stu-id="7275f-202">See also</span></span>

- [<span data-ttu-id="7275f-203">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7275f-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7275f-204">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="7275f-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7275f-205">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="7275f-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

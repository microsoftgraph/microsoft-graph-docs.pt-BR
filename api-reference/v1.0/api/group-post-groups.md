---
title: Criar grupo
description: 'Use esta API para criar um novo grupo, conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8bf432d30ba000641654d8c5d457096f5bfcb70e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574863"
---
# <a name="create-group"></a><span data-ttu-id="e2612-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="e2612-104">Create group</span></span>
<span data-ttu-id="e2612-p102">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="e2612-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="e2612-107">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="e2612-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="e2612-108">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="e2612-108">Dynamic group</span></span>
* <span data-ttu-id="e2612-109">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="e2612-109">Security group</span></span>

<span data-ttu-id="e2612-110">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="e2612-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e2612-111">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="e2612-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="e2612-112">Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="e2612-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="e2612-113">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="e2612-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="e2612-p105">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e2612-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2612-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2612-116">Permissions</span></span>
<span data-ttu-id="e2612-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2612-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2612-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2612-119">Permission type</span></span>      | <span data-ttu-id="e2612-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2612-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2612-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2612-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e2612-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2612-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2612-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2612-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2612-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2612-124">Not supported.</span></span>    |
|<span data-ttu-id="e2612-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2612-125">Application</span></span> | <span data-ttu-id="e2612-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2612-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2612-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2612-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="e2612-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2612-128">Request headers</span></span>
| <span data-ttu-id="e2612-129">Nome</span><span class="sxs-lookup"><span data-stu-id="e2612-129">Name</span></span>       | <span data-ttu-id="e2612-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2612-130">Type</span></span> | <span data-ttu-id="e2612-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2612-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2612-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2612-132">Authorization</span></span>  | <span data-ttu-id="e2612-133">string</span><span class="sxs-lookup"><span data-stu-id="e2612-133">string</span></span>  | <span data-ttu-id="e2612-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2612-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2612-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2612-136">Content-Type</span></span>  | <span data-ttu-id="e2612-137">application/json</span><span class="sxs-lookup"><span data-stu-id="e2612-137">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2612-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2612-138">Request body</span></span>
<span data-ttu-id="e2612-139">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="e2612-139">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="e2612-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2612-140">Property</span></span> | <span data-ttu-id="e2612-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2612-141">Type</span></span> | <span data-ttu-id="e2612-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2612-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2612-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e2612-143">displayName</span></span> | <span data-ttu-id="e2612-144">string</span><span class="sxs-lookup"><span data-stu-id="e2612-144">string</span></span> | <span data-ttu-id="e2612-145">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="e2612-145">The name to display in the address book for the group.</span></span> <span data-ttu-id="e2612-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2612-146">Required.</span></span> |
| <span data-ttu-id="e2612-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e2612-147">mailEnabled</span></span> | <span data-ttu-id="e2612-148">booliano</span><span class="sxs-lookup"><span data-stu-id="e2612-148">boolean</span></span> | <span data-ttu-id="e2612-149">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="e2612-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="e2612-150">Defina isto como **true**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e2612-150">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="e2612-151">Defina como **false**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="e2612-151">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="e2612-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2612-152">Required.</span></span> |
| <span data-ttu-id="e2612-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e2612-153">mailNickname</span></span> | <span data-ttu-id="e2612-154">string</span><span class="sxs-lookup"><span data-stu-id="e2612-154">string</span></span> | <span data-ttu-id="e2612-155">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="e2612-155">The mail alias for the group.</span></span> <span data-ttu-id="e2612-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2612-156">Required.</span></span> |
| <span data-ttu-id="e2612-157">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e2612-157">securityEnabled</span></span> | <span data-ttu-id="e2612-158">booliano</span><span class="sxs-lookup"><span data-stu-id="e2612-158">boolean</span></span> | <span data-ttu-id="e2612-159">Defina como **true** para grupos habilitados para segurança.</span><span class="sxs-lookup"><span data-stu-id="e2612-159">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="e2612-160">Definir isto como **true**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="e2612-160">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="e2612-161">Defina isto como **false**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e2612-161">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="e2612-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2612-162">Required.</span></span> |
| <span data-ttu-id="e2612-163">owners</span><span class="sxs-lookup"><span data-stu-id="e2612-163">owners</span></span> | <span data-ttu-id="e2612-164">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2612-164">string collection</span></span> | <span data-ttu-id="e2612-165">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="e2612-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="e2612-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e2612-166">Optional.</span></span> |
| <span data-ttu-id="e2612-167">membros</span><span class="sxs-lookup"><span data-stu-id="e2612-167">members</span></span> | <span data-ttu-id="e2612-168">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2612-168">string collection</span></span> | <span data-ttu-id="e2612-169">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="e2612-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="e2612-170">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e2612-170">Optional.</span></span> |


<span data-ttu-id="e2612-171">Especifique a propriedade **groupTypes**, se estiver criando um Grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="e2612-171">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="e2612-172">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="e2612-172">groupTypes options</span></span>

| <span data-ttu-id="e2612-173">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="e2612-173">Type of group</span></span> | <span data-ttu-id="e2612-174">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="e2612-174">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="e2612-175">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="e2612-175">Office 365 (aka unified group)</span></span>| <span data-ttu-id="e2612-176">"Unified"</span><span class="sxs-lookup"><span data-stu-id="e2612-176">"Unified"</span></span> |
| <span data-ttu-id="e2612-177">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="e2612-177">Dynamic</span></span> | <span data-ttu-id="e2612-178">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="e2612-178">"DynamicMembership"</span></span> |
| <span data-ttu-id="e2612-179">Segurança</span><span class="sxs-lookup"><span data-stu-id="e2612-179">Security</span></span> | <span data-ttu-id="e2612-180">Não defina.</span><span class="sxs-lookup"><span data-stu-id="e2612-180">Do not set.</span></span> |


><span data-ttu-id="e2612-181">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="e2612-181">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="e2612-182">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="e2612-182">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="e2612-p115">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="e2612-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="e2612-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2612-185">Response</span></span>
<span data-ttu-id="e2612-186">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2612-186">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e2612-187">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="e2612-187">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="e2612-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2612-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e2612-189">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e2612-189">Request 1</span></span>
<span data-ttu-id="e2612-190">A primeira solicitação de exemplo cria um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e2612-190">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="e2612-191">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e2612-191">Response 1</span></span>
<span data-ttu-id="e2612-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2612-192">The following is an example of the response.</span></span>
><span data-ttu-id="e2612-193">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2612-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2612-194">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2612-194">All the default properties are returned from an actual call.</span></span>
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
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T00:51:37Z",
      "creationOptions": [],
      "description": "Self help community for library",
      "displayName": "Library Assist",
      "groupTypes": [
          "Unified"
      ],
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="e2612-195">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e2612-195">Request 2</span></span>
<span data-ttu-id="e2612-196">A segunda solicitação de exemplo cria um Grupo do Office 365 com um proprietário especificado.</span><span class="sxs-lookup"><span data-stu-id="e2612-196">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
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
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="e2612-197">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e2612-197">Response 2</span></span>
<span data-ttu-id="e2612-198">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="e2612-198">The following is an example of a successful response.</span></span> <span data-ttu-id="e2612-199">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="e2612-199">It includes only default properties.</span></span> <span data-ttu-id="e2612-200">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="e2612-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="e2612-201">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2612-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2612-202">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2612-202">All the default properties are returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

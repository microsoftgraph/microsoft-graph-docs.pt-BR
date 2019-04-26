---
title: Criar grupo
description: 'Use esta API para criar um novo grupo, conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8bf432d30ba000641654d8c5d457096f5bfcb70e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561793"
---
# <a name="create-group"></a><span data-ttu-id="70515-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="70515-104">Create group</span></span>
<span data-ttu-id="70515-p102">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="70515-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="70515-107">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="70515-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="70515-108">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="70515-108">Dynamic group</span></span>
* <span data-ttu-id="70515-109">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="70515-109">Security group</span></span>

<span data-ttu-id="70515-110">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="70515-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="70515-111">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="70515-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="70515-112">Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="70515-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="70515-113">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="70515-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="70515-p105">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="70515-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="70515-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="70515-116">Permissions</span></span>
<span data-ttu-id="70515-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70515-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70515-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70515-119">Permission type</span></span>      | <span data-ttu-id="70515-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70515-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70515-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70515-121">Delegated (work or school account)</span></span> | <span data-ttu-id="70515-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70515-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="70515-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70515-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70515-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70515-124">Not supported.</span></span>    |
|<span data-ttu-id="70515-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70515-125">Application</span></span> | <span data-ttu-id="70515-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70515-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70515-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70515-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="70515-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70515-128">Request headers</span></span>
| <span data-ttu-id="70515-129">Nome</span><span class="sxs-lookup"><span data-stu-id="70515-129">Name</span></span>       | <span data-ttu-id="70515-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="70515-130">Type</span></span> | <span data-ttu-id="70515-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="70515-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70515-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="70515-132">Authorization</span></span>  | <span data-ttu-id="70515-133">string</span><span class="sxs-lookup"><span data-stu-id="70515-133">string</span></span>  | <span data-ttu-id="70515-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70515-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70515-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70515-136">Content-Type</span></span>  | <span data-ttu-id="70515-137">application/json</span><span class="sxs-lookup"><span data-stu-id="70515-137">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70515-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70515-138">Request body</span></span>
<span data-ttu-id="70515-139">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="70515-139">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="70515-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70515-140">Property</span></span> | <span data-ttu-id="70515-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="70515-141">Type</span></span> | <span data-ttu-id="70515-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="70515-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70515-143">displayName</span><span class="sxs-lookup"><span data-stu-id="70515-143">displayName</span></span> | <span data-ttu-id="70515-144">string</span><span class="sxs-lookup"><span data-stu-id="70515-144">string</span></span> | <span data-ttu-id="70515-145">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="70515-145">The name to display in the address book for the group.</span></span> <span data-ttu-id="70515-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70515-146">Required.</span></span> |
| <span data-ttu-id="70515-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="70515-147">mailEnabled</span></span> | <span data-ttu-id="70515-148">booliano</span><span class="sxs-lookup"><span data-stu-id="70515-148">boolean</span></span> | <span data-ttu-id="70515-149">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="70515-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="70515-150">Defina isto como **true**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="70515-150">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="70515-151">Defina como **false**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="70515-151">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="70515-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70515-152">Required.</span></span> |
| <span data-ttu-id="70515-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="70515-153">mailNickname</span></span> | <span data-ttu-id="70515-154">string</span><span class="sxs-lookup"><span data-stu-id="70515-154">string</span></span> | <span data-ttu-id="70515-155">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="70515-155">The mail alias for the group.</span></span> <span data-ttu-id="70515-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70515-156">Required.</span></span> |
| <span data-ttu-id="70515-157">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="70515-157">securityEnabled</span></span> | <span data-ttu-id="70515-158">booliano</span><span class="sxs-lookup"><span data-stu-id="70515-158">boolean</span></span> | <span data-ttu-id="70515-159">Defina como **true** para grupos habilitados para segurança.</span><span class="sxs-lookup"><span data-stu-id="70515-159">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="70515-160">Definir isto como **true**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="70515-160">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="70515-161">Defina isto como **false**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="70515-161">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="70515-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70515-162">Required.</span></span> |
| <span data-ttu-id="70515-163">owners</span><span class="sxs-lookup"><span data-stu-id="70515-163">owners</span></span> | <span data-ttu-id="70515-164">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70515-164">string collection</span></span> | <span data-ttu-id="70515-165">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="70515-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="70515-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70515-166">Optional.</span></span> |
| <span data-ttu-id="70515-167">membros</span><span class="sxs-lookup"><span data-stu-id="70515-167">members</span></span> | <span data-ttu-id="70515-168">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70515-168">string collection</span></span> | <span data-ttu-id="70515-169">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="70515-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="70515-170">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70515-170">Optional.</span></span> |


<span data-ttu-id="70515-171">Especifique a propriedade **groupTypes**, se estiver criando um Grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="70515-171">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="70515-172">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="70515-172">groupTypes options</span></span>

| <span data-ttu-id="70515-173">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="70515-173">Type of group</span></span> | <span data-ttu-id="70515-174">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="70515-174">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="70515-175">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="70515-175">Office 365 (aka unified group)</span></span>| <span data-ttu-id="70515-176">"Unified"</span><span class="sxs-lookup"><span data-stu-id="70515-176">"Unified"</span></span> |
| <span data-ttu-id="70515-177">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="70515-177">Dynamic</span></span> | <span data-ttu-id="70515-178">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="70515-178">"DynamicMembership"</span></span> |
| <span data-ttu-id="70515-179">Segurança</span><span class="sxs-lookup"><span data-stu-id="70515-179">Security</span></span> | <span data-ttu-id="70515-180">Não defina.</span><span class="sxs-lookup"><span data-stu-id="70515-180">Do not set.</span></span> |


><span data-ttu-id="70515-181">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="70515-181">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="70515-182">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="70515-182">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="70515-p115">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="70515-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="70515-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="70515-185">Response</span></span>
<span data-ttu-id="70515-186">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70515-186">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="70515-187">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="70515-187">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="70515-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70515-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="70515-189">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="70515-189">Request 1</span></span>
<span data-ttu-id="70515-190">A primeira solicitação de exemplo cria um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="70515-190">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="70515-191">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="70515-191">Response 1</span></span>
<span data-ttu-id="70515-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70515-192">The following is an example of the response.</span></span>
><span data-ttu-id="70515-193">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70515-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="70515-194">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70515-194">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="70515-195">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="70515-195">Request 2</span></span>
<span data-ttu-id="70515-196">A segunda solicitação de exemplo cria um Grupo do Office 365 com um proprietário especificado.</span><span class="sxs-lookup"><span data-stu-id="70515-196">The second example request creates an Office 365 group with an owner and members specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="70515-197">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="70515-197">Response 2</span></span>
<span data-ttu-id="70515-198">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="70515-198">The following is an example of a successful response.</span></span> <span data-ttu-id="70515-199">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="70515-199">It includes only default properties.</span></span> <span data-ttu-id="70515-200">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="70515-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="70515-201">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70515-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="70515-202">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70515-202">All the default properties are returned from an actual call.</span></span>
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

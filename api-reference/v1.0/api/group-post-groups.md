---
title: Criar grupo
description: 'Crie um novo grupo conforme especificado no corpo da solicitação. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: baaf76455fefc6e44bf4995854d99baafb713005
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036371"
---
# <a name="create-group"></a><span data-ttu-id="26919-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="26919-103">Create group</span></span>
<span data-ttu-id="26919-104">Crie um novo grupo conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26919-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="26919-105">Você pode criar os seguintes tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="26919-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="26919-106">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="26919-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="26919-107">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="26919-107">Security group</span></span>

<span data-ttu-id="26919-108">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="26919-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="26919-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="26919-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="26919-110">Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="26919-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="26919-111">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="26919-111">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="26919-p104">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="26919-p104">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="26919-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="26919-114">Permissions</span></span>
<span data-ttu-id="26919-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26919-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26919-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26919-117">Permission type</span></span>      | <span data-ttu-id="26919-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26919-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26919-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26919-119">Delegated (work or school account)</span></span> | <span data-ttu-id="26919-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26919-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="26919-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26919-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26919-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26919-122">Not supported.</span></span>    |
|<span data-ttu-id="26919-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26919-123">Application</span></span> | <span data-ttu-id="26919-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26919-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26919-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26919-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="26919-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26919-126">Request headers</span></span>
| <span data-ttu-id="26919-127">Nome</span><span class="sxs-lookup"><span data-stu-id="26919-127">Name</span></span>       | <span data-ttu-id="26919-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="26919-128">Type</span></span> | <span data-ttu-id="26919-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="26919-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26919-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="26919-130">Authorization</span></span>  | <span data-ttu-id="26919-131">string</span><span class="sxs-lookup"><span data-stu-id="26919-131">string</span></span>  | <span data-ttu-id="26919-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26919-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26919-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26919-134">Content-Type</span></span>  | <span data-ttu-id="26919-135">application/json</span><span class="sxs-lookup"><span data-stu-id="26919-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26919-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26919-136">Request body</span></span>
<span data-ttu-id="26919-137">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="26919-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="26919-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26919-138">Property</span></span> | <span data-ttu-id="26919-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="26919-139">Type</span></span> | <span data-ttu-id="26919-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="26919-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26919-141">displayName</span><span class="sxs-lookup"><span data-stu-id="26919-141">displayName</span></span> | <span data-ttu-id="26919-142">string</span><span class="sxs-lookup"><span data-stu-id="26919-142">string</span></span> | <span data-ttu-id="26919-143">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="26919-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="26919-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26919-144">Required.</span></span> |
| <span data-ttu-id="26919-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="26919-145">mailEnabled</span></span> | <span data-ttu-id="26919-146">booliano</span><span class="sxs-lookup"><span data-stu-id="26919-146">boolean</span></span> | <span data-ttu-id="26919-147">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="26919-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="26919-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26919-148">Required.</span></span> |
| <span data-ttu-id="26919-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="26919-149">mailNickname</span></span> | <span data-ttu-id="26919-150">string</span><span class="sxs-lookup"><span data-stu-id="26919-150">string</span></span> | <span data-ttu-id="26919-151">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="26919-151">The mail alias for the group.</span></span> <span data-ttu-id="26919-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26919-152">Required.</span></span> |
| <span data-ttu-id="26919-153">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="26919-153">securityEnabled</span></span> | <span data-ttu-id="26919-154">booliano</span><span class="sxs-lookup"><span data-stu-id="26919-154">boolean</span></span> | <span data-ttu-id="26919-155">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="26919-155">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="26919-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26919-156">Required.</span></span> |
| <span data-ttu-id="26919-157">owners</span><span class="sxs-lookup"><span data-stu-id="26919-157">owners</span></span> | <span data-ttu-id="26919-158">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26919-158">string collection</span></span> | <span data-ttu-id="26919-159">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="26919-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="26919-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="26919-160">Optional.</span></span> |
| <span data-ttu-id="26919-161">membros</span><span class="sxs-lookup"><span data-stu-id="26919-161">members</span></span> | <span data-ttu-id="26919-162">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26919-162">string collection</span></span> | <span data-ttu-id="26919-163">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="26919-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="26919-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="26919-164">Optional.</span></span> |

> <span data-ttu-id="26919-165">Observação: Os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** e **mailEnabled** definidos inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="26919-165">Note: Groups created using the Microsoft Azure portal always have **securityEnabled** and **mailEnabled** initially set to `true`.</span></span>

<span data-ttu-id="26919-166">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="26919-166">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="26919-167">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="26919-167">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="26919-168">**Observação:** Criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="26919-168">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="26919-169">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="26919-169">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="26919-170">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="26919-170">groupTypes options</span></span>

<span data-ttu-id="26919-171">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrado abaixo:</span><span class="sxs-lookup"><span data-stu-id="26919-171">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="26919-172">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="26919-172">Type of group</span></span> | <span data-ttu-id="26919-173">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="26919-173">Assigned membership</span></span> | <span data-ttu-id="26919-174">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="26919-174">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="26919-175">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="26919-175">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="26919-176">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="26919-176">Dynamic</span></span> | <span data-ttu-id="26919-177">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="26919-177">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="26919-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="26919-178">Response</span></span>
<span data-ttu-id="26919-179">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26919-179">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="26919-180">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="26919-180">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="26919-181">Exemplos</span><span class="sxs-lookup"><span data-stu-id="26919-181">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="26919-182">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="26919-182">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="26919-183">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="26919-183">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="26919-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26919-184">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="26919-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="26919-185">Response</span></span>

<span data-ttu-id="26919-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="26919-186">The following is an example of the response.</span></span>

><span data-ttu-id="26919-187">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26919-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="26919-188">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26919-188">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="26919-189">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="26919-189">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="26919-190">C#</span><span class="sxs-lookup"><span data-stu-id="26919-190">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26919-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="26919-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="26919-192">Exemplo 2: Criando um grupo com membros e proprietários</span><span class="sxs-lookup"><span data-stu-id="26919-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="26919-193">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="26919-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="26919-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26919-194">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="26919-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="26919-195">Response</span></span>

<span data-ttu-id="26919-196">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="26919-196">The following is an example of a successful response.</span></span> <span data-ttu-id="26919-197">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="26919-197">It includes only default properties.</span></span> <span data-ttu-id="26919-198">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="26919-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="26919-199">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26919-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="26919-200">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26919-200">All the default properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="26919-201">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="26919-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="26919-202">C#</span><span class="sxs-lookup"><span data-stu-id="26919-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26919-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="26919-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

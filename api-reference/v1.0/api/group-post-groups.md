---
title: Criar grupo
description: 'Crie um novo grupo conforme especificado no corpo da solicitação. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: ff8d4c28e4b2fed0858650d704dca34feb8eb79a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277781"
---
# <a name="create-group"></a><span data-ttu-id="cfcbf-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="cfcbf-103">Create group</span></span>
<span data-ttu-id="cfcbf-104">Crie um novo grupo conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="cfcbf-105">Você pode criar os seguintes tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="cfcbf-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="cfcbf-106">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="cfcbf-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="cfcbf-107">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="cfcbf-107">Security group</span></span>

<span data-ttu-id="cfcbf-108">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="cfcbf-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="cfcbf-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="cfcbf-110">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="cfcbf-p103">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfcbf-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfcbf-113">Permissions</span></span>
<span data-ttu-id="cfcbf-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfcbf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfcbf-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfcbf-116">Permission type</span></span>      | <span data-ttu-id="cfcbf-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfcbf-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfcbf-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfcbf-118">Delegated (work or school account)</span></span> | <span data-ttu-id="cfcbf-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfcbf-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="cfcbf-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfcbf-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfcbf-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-121">Not supported.</span></span>    |
|<span data-ttu-id="cfcbf-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfcbf-122">Application</span></span> | <span data-ttu-id="cfcbf-123">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfcbf-123">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfcbf-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfcbf-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="cfcbf-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfcbf-125">Request headers</span></span>
| <span data-ttu-id="cfcbf-126">Nome</span><span class="sxs-lookup"><span data-stu-id="cfcbf-126">Name</span></span>       | <span data-ttu-id="cfcbf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfcbf-127">Type</span></span> | <span data-ttu-id="cfcbf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfcbf-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfcbf-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfcbf-129">Authorization</span></span>  | <span data-ttu-id="cfcbf-130">string</span><span class="sxs-lookup"><span data-stu-id="cfcbf-130">string</span></span>  | <span data-ttu-id="cfcbf-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfcbf-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfcbf-133">Content-Type</span></span>  | <span data-ttu-id="cfcbf-134">application/json</span><span class="sxs-lookup"><span data-stu-id="cfcbf-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfcbf-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfcbf-135">Request body</span></span>
<span data-ttu-id="cfcbf-136">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="cfcbf-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfcbf-137">Property</span></span> | <span data-ttu-id="cfcbf-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfcbf-138">Type</span></span> | <span data-ttu-id="cfcbf-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfcbf-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfcbf-140">displayName</span><span class="sxs-lookup"><span data-stu-id="cfcbf-140">displayName</span></span> | <span data-ttu-id="cfcbf-141">string</span><span class="sxs-lookup"><span data-stu-id="cfcbf-141">string</span></span> | <span data-ttu-id="cfcbf-142">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="cfcbf-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-143">Required.</span></span> |
| <span data-ttu-id="cfcbf-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="cfcbf-144">mailEnabled</span></span> | <span data-ttu-id="cfcbf-145">booliano</span><span class="sxs-lookup"><span data-stu-id="cfcbf-145">boolean</span></span> | <span data-ttu-id="cfcbf-146">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="cfcbf-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-147">Required.</span></span> |
| <span data-ttu-id="cfcbf-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cfcbf-148">mailNickname</span></span> | <span data-ttu-id="cfcbf-149">string</span><span class="sxs-lookup"><span data-stu-id="cfcbf-149">string</span></span> | <span data-ttu-id="cfcbf-150">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-150">The mail alias for the group.</span></span> <span data-ttu-id="cfcbf-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-151">Required.</span></span> |
| <span data-ttu-id="cfcbf-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="cfcbf-152">securityEnabled</span></span> | <span data-ttu-id="cfcbf-153">booliano</span><span class="sxs-lookup"><span data-stu-id="cfcbf-153">boolean</span></span> | <span data-ttu-id="cfcbf-154">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="cfcbf-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-155">Required.</span></span> |
| <span data-ttu-id="cfcbf-156">owners</span><span class="sxs-lookup"><span data-stu-id="cfcbf-156">owners</span></span> | <span data-ttu-id="cfcbf-157">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfcbf-157">string collection</span></span> | <span data-ttu-id="cfcbf-158">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="cfcbf-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-159">Optional.</span></span> |
| <span data-ttu-id="cfcbf-160">membros</span><span class="sxs-lookup"><span data-stu-id="cfcbf-160">members</span></span> | <span data-ttu-id="cfcbf-161">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfcbf-161">string collection</span></span> | <span data-ttu-id="cfcbf-162">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="cfcbf-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-163">Optional.</span></span> |

> <span data-ttu-id="cfcbf-164">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="cfcbf-165">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="cfcbf-166">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="cfcbf-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="cfcbf-167">**Observação:** Criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-167">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="cfcbf-168">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-168">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="cfcbf-169">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="cfcbf-169">groupTypes options</span></span>

<span data-ttu-id="cfcbf-170">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrado abaixo:</span><span class="sxs-lookup"><span data-stu-id="cfcbf-170">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="cfcbf-171">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="cfcbf-171">Type of group</span></span> | <span data-ttu-id="cfcbf-172">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="cfcbf-172">Assigned membership</span></span> | <span data-ttu-id="cfcbf-173">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="cfcbf-173">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="cfcbf-174">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="cfcbf-174">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="cfcbf-175">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="cfcbf-175">Dynamic</span></span> | <span data-ttu-id="cfcbf-176">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="cfcbf-176">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="cfcbf-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfcbf-177">Response</span></span>
<span data-ttu-id="cfcbf-178">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-178">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="cfcbf-179">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-179">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="cfcbf-180">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cfcbf-180">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="cfcbf-181">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="cfcbf-181">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="cfcbf-182">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-182">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="cfcbf-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfcbf-183">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cfcbf-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfcbf-184">Response</span></span>

<span data-ttu-id="cfcbf-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-185">The following is an example of the response.</span></span>

><span data-ttu-id="cfcbf-186">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cfcbf-187">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-187">All the default properties are returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cfcbf-188">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="cfcbf-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cfcbf-189">C#</span><span class="sxs-lookup"><span data-stu-id="cfcbf-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfcbf-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfcbf-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cfcbf-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfcbf-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="cfcbf-192">Exemplo 2: criando um grupo com membros e proprietários</span><span class="sxs-lookup"><span data-stu-id="cfcbf-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="cfcbf-193">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="cfcbf-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfcbf-194">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cfcbf-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfcbf-195">Response</span></span>

<span data-ttu-id="cfcbf-196">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-196">The following is an example of a successful response.</span></span> <span data-ttu-id="cfcbf-197">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-197">It includes only default properties.</span></span> <span data-ttu-id="cfcbf-198">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="cfcbf-199">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cfcbf-200">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfcbf-200">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cfcbf-201">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="cfcbf-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cfcbf-202">C#</span><span class="sxs-lookup"><span data-stu-id="cfcbf-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfcbf-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfcbf-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cfcbf-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfcbf-204">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

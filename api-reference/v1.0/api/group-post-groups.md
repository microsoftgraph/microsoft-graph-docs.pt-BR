---
title: Criar grupo
description: 'Crie um novo grupo conforme especificado no corpo da solicitação. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: f6b911e0e3e602ce96c10cab22a27ed26788df6e
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820602"
---
# <a name="create-group"></a><span data-ttu-id="355f7-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="355f7-103">Create group</span></span>
<span data-ttu-id="355f7-104">Crie um novo grupo conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="355f7-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="355f7-105">Você pode criar os seguintes tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="355f7-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="355f7-106">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="355f7-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="355f7-107">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="355f7-107">Security group</span></span>

<span data-ttu-id="355f7-108">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="355f7-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="355f7-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="355f7-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="355f7-110">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta do `$select` OData.</span><span class="sxs-lookup"><span data-stu-id="355f7-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="355f7-111">**Observação**: Embora o Microsoft Teams tenha como base grupos do Office 365, atualmente não é possível criar uma equipe por meio desta API.</span><span class="sxs-lookup"><span data-stu-id="355f7-111">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span> <span data-ttu-id="355f7-112">Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="355f7-112">Note: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="355f7-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="355f7-113">Permissions</span></span>
<span data-ttu-id="355f7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="355f7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="355f7-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="355f7-116">Permission type</span></span>      | <span data-ttu-id="355f7-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="355f7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="355f7-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="355f7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="355f7-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="355f7-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="355f7-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="355f7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="355f7-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="355f7-121">Not supported.</span></span>    |
|<span data-ttu-id="355f7-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="355f7-122">Application</span></span> | <span data-ttu-id="355f7-123">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="355f7-123">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="355f7-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="355f7-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="355f7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="355f7-125">Request headers</span></span>
| <span data-ttu-id="355f7-126">Nome</span><span class="sxs-lookup"><span data-stu-id="355f7-126">Name</span></span>       | <span data-ttu-id="355f7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="355f7-127">Type</span></span> | <span data-ttu-id="355f7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="355f7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="355f7-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="355f7-129">Authorization</span></span>  | <span data-ttu-id="355f7-130">string</span><span class="sxs-lookup"><span data-stu-id="355f7-130">string</span></span>  | <span data-ttu-id="355f7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="355f7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="355f7-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="355f7-133">Content-Type</span></span>  | <span data-ttu-id="355f7-134">application/json</span><span class="sxs-lookup"><span data-stu-id="355f7-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="355f7-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="355f7-135">Request body</span></span>
<span data-ttu-id="355f7-136">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="355f7-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="355f7-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="355f7-137">Property</span></span> | <span data-ttu-id="355f7-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="355f7-138">Type</span></span> | <span data-ttu-id="355f7-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="355f7-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="355f7-140">displayName</span><span class="sxs-lookup"><span data-stu-id="355f7-140">displayName</span></span> | <span data-ttu-id="355f7-141">string</span><span class="sxs-lookup"><span data-stu-id="355f7-141">string</span></span> | <span data-ttu-id="355f7-142">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="355f7-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="355f7-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="355f7-143">Required.</span></span> |
| <span data-ttu-id="355f7-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="355f7-144">mailEnabled</span></span> | <span data-ttu-id="355f7-145">booliano</span><span class="sxs-lookup"><span data-stu-id="355f7-145">boolean</span></span> | <span data-ttu-id="355f7-146">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="355f7-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="355f7-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="355f7-147">Required.</span></span> |
| <span data-ttu-id="355f7-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="355f7-148">mailNickname</span></span> | <span data-ttu-id="355f7-149">string</span><span class="sxs-lookup"><span data-stu-id="355f7-149">string</span></span> | <span data-ttu-id="355f7-150">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="355f7-150">The mail alias for the group.</span></span> <span data-ttu-id="355f7-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="355f7-151">Required.</span></span> |
| <span data-ttu-id="355f7-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="355f7-152">securityEnabled</span></span> | <span data-ttu-id="355f7-153">booliano</span><span class="sxs-lookup"><span data-stu-id="355f7-153">boolean</span></span> | <span data-ttu-id="355f7-154">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="355f7-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="355f7-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="355f7-155">Required.</span></span> |
| <span data-ttu-id="355f7-156">owners</span><span class="sxs-lookup"><span data-stu-id="355f7-156">owners</span></span> | <span data-ttu-id="355f7-157">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="355f7-157">string collection</span></span> | <span data-ttu-id="355f7-158">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="355f7-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="355f7-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="355f7-159">Optional.</span></span> |
| <span data-ttu-id="355f7-160">membros</span><span class="sxs-lookup"><span data-stu-id="355f7-160">members</span></span> | <span data-ttu-id="355f7-161">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="355f7-161">string collection</span></span> | <span data-ttu-id="355f7-162">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="355f7-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="355f7-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="355f7-163">Optional.</span></span> |

> <span data-ttu-id="355f7-164">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="355f7-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="355f7-165">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="355f7-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="355f7-166">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="355f7-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="355f7-167">**Observação:** Criar um Grupo do Office 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="355f7-167">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="355f7-168">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="355f7-168">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="355f7-169">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="355f7-169">groupTypes options</span></span>

<span data-ttu-id="355f7-170">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="355f7-170">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="355f7-171">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="355f7-171">Type of group</span></span> | <span data-ttu-id="355f7-172">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="355f7-172">Assigned membership</span></span> | <span data-ttu-id="355f7-173">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="355f7-173">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="355f7-174">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="355f7-174">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="355f7-175">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="355f7-175">Dynamic</span></span> | <span data-ttu-id="355f7-176">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="355f7-176">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="355f7-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="355f7-177">Response</span></span>
<span data-ttu-id="355f7-178">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="355f7-178">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="355f7-179">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="355f7-179">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="355f7-180">Exemplos</span><span class="sxs-lookup"><span data-stu-id="355f7-180">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="355f7-181">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="355f7-181">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="355f7-182">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="355f7-182">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="355f7-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="355f7-183">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="355f7-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="355f7-184">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="355f7-185">C#</span><span class="sxs-lookup"><span data-stu-id="355f7-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="355f7-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="355f7-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="355f7-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="355f7-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="355f7-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="355f7-188">Response</span></span>

<span data-ttu-id="355f7-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="355f7-189">The following is an example of the response.</span></span>

><span data-ttu-id="355f7-190">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="355f7-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="355f7-191">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="355f7-191">All the default properties are returned from an actual call.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="355f7-192">Exemplo 2: criando um grupo com membros e proprietários</span><span class="sxs-lookup"><span data-stu-id="355f7-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="355f7-193">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="355f7-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="355f7-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="355f7-194">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="355f7-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="355f7-195">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="355f7-196">C#</span><span class="sxs-lookup"><span data-stu-id="355f7-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="355f7-197">Javascript</span><span class="sxs-lookup"><span data-stu-id="355f7-197">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="355f7-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="355f7-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="355f7-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="355f7-199">Response</span></span>

<span data-ttu-id="355f7-200">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="355f7-200">The following is an example of a successful response.</span></span> <span data-ttu-id="355f7-201">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="355f7-201">It includes only default properties.</span></span> <span data-ttu-id="355f7-202">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="355f7-202">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="355f7-203">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="355f7-203">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="355f7-204">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="355f7-204">All the default properties are returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

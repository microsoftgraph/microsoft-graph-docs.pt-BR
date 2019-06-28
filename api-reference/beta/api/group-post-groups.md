---
title: Criar grupo
description: Crie um novo grupo ou grupo de segurança do Office 365.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 918e1b40ff45b92b44d3e18970f232cd318a2865
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262941"
---
# <a name="create-group"></a><span data-ttu-id="58d9e-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="58d9e-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58d9e-104">Crie um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58d9e-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="58d9e-105">Você pode criar um dos seguintes grupos:</span><span class="sxs-lookup"><span data-stu-id="58d9e-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="58d9e-106">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="58d9e-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="58d9e-107">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="58d9e-107">Security group</span></span>

<span data-ttu-id="58d9e-108">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="58d9e-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="58d9e-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="58d9e-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="58d9e-110">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="58d9e-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="58d9e-111">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="58d9e-111">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58d9e-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="58d9e-112">Permissions</span></span>
<span data-ttu-id="58d9e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58d9e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58d9e-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58d9e-115">Permission type</span></span>      | <span data-ttu-id="58d9e-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58d9e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58d9e-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58d9e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="58d9e-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58d9e-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="58d9e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58d9e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58d9e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58d9e-120">Not supported.</span></span>    |
|<span data-ttu-id="58d9e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58d9e-121">Application</span></span> | <span data-ttu-id="58d9e-122">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d9e-122">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58d9e-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58d9e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="58d9e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9e-124">Request headers</span></span>

| <span data-ttu-id="58d9e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="58d9e-125">Name</span></span>       | <span data-ttu-id="58d9e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="58d9e-126">Type</span></span> | <span data-ttu-id="58d9e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d9e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58d9e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="58d9e-128">Authorization</span></span>  | <span data-ttu-id="58d9e-129">string</span><span class="sxs-lookup"><span data-stu-id="58d9e-129">string</span></span>  | <span data-ttu-id="58d9e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58d9e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58d9e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9e-132">Request body</span></span>

<span data-ttu-id="58d9e-133">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="58d9e-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="58d9e-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58d9e-134">Property</span></span> | <span data-ttu-id="58d9e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="58d9e-135">Type</span></span> | <span data-ttu-id="58d9e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d9e-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58d9e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="58d9e-137">displayName</span></span> | <span data-ttu-id="58d9e-138">string</span><span class="sxs-lookup"><span data-stu-id="58d9e-138">string</span></span> | <span data-ttu-id="58d9e-139">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="58d9e-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="58d9e-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58d9e-140">Required.</span></span> |
| <span data-ttu-id="58d9e-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="58d9e-141">mailEnabled</span></span> | <span data-ttu-id="58d9e-142">booliano</span><span class="sxs-lookup"><span data-stu-id="58d9e-142">boolean</span></span> | <span data-ttu-id="58d9e-143">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="58d9e-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="58d9e-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58d9e-144">Required.</span></span> |
| <span data-ttu-id="58d9e-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="58d9e-145">mailNickname</span></span> | <span data-ttu-id="58d9e-146">string</span><span class="sxs-lookup"><span data-stu-id="58d9e-146">string</span></span> | <span data-ttu-id="58d9e-147">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="58d9e-147">The mail alias for the group.</span></span> <span data-ttu-id="58d9e-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58d9e-148">Required.</span></span> |
| <span data-ttu-id="58d9e-149">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="58d9e-149">securityEnabled</span></span> | <span data-ttu-id="58d9e-150">booliano</span><span class="sxs-lookup"><span data-stu-id="58d9e-150">boolean</span></span> | <span data-ttu-id="58d9e-151">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="58d9e-151">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="58d9e-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58d9e-152">Required.</span></span> |
| <span data-ttu-id="58d9e-153">owners</span><span class="sxs-lookup"><span data-stu-id="58d9e-153">owners</span></span> | <span data-ttu-id="58d9e-154">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="58d9e-154">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="58d9e-155">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="58d9e-155">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="58d9e-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58d9e-156">Optional.</span></span> |
| <span data-ttu-id="58d9e-157">membros</span><span class="sxs-lookup"><span data-stu-id="58d9e-157">members</span></span> | <span data-ttu-id="58d9e-158">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="58d9e-158">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="58d9e-159">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="58d9e-159">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="58d9e-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58d9e-160">Optional.</span></span> |

> <span data-ttu-id="58d9e-161">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="58d9e-161">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="58d9e-162">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="58d9e-162">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="58d9e-163">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="58d9e-163">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="58d9e-164">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="58d9e-164">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="58d9e-p112">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="58d9e-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="58d9e-167">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="58d9e-167">groupTypes options</span></span>

<span data-ttu-id="58d9e-168">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrado abaixo:</span><span class="sxs-lookup"><span data-stu-id="58d9e-168">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="58d9e-169">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="58d9e-169">Type of group</span></span> | <span data-ttu-id="58d9e-170">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="58d9e-170">Assigned membership</span></span> | <span data-ttu-id="58d9e-171">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="58d9e-171">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="58d9e-172">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="58d9e-172">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="58d9e-173">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="58d9e-173">Dynamic</span></span> | <span data-ttu-id="58d9e-174">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="58d9e-174">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="58d9e-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="58d9e-175">Response</span></span>

<span data-ttu-id="58d9e-176">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58d9e-176">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="58d9e-177">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="58d9e-177">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="58d9e-178">Exemplos</span><span class="sxs-lookup"><span data-stu-id="58d9e-178">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="58d9e-179">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="58d9e-179">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="58d9e-180">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="58d9e-180">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="58d9e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9e-181">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="58d9e-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="58d9e-182">Response</span></span>

<span data-ttu-id="58d9e-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58d9e-183">The following is an example of the response.</span></span>

><span data-ttu-id="58d9e-184">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58d9e-184">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="58d9e-185">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58d9e-185">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="58d9e-186">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="58d9e-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="58d9e-187">C#</span><span class="sxs-lookup"><span data-stu-id="58d9e-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58d9e-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="58d9e-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="58d9e-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58d9e-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="58d9e-190">Exemplo 2: criando um grupo do Office 365 com um proprietário e membros</span><span class="sxs-lookup"><span data-stu-id="58d9e-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="58d9e-191">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="58d9e-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="58d9e-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9e-192">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="58d9e-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="58d9e-193">Response</span></span> 

<span data-ttu-id="58d9e-194">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="58d9e-194">The following is an example of a successful response.</span></span> <span data-ttu-id="58d9e-195">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="58d9e-195">It includes only default properties.</span></span> <span data-ttu-id="58d9e-196">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="58d9e-196">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="58d9e-197">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58d9e-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="58d9e-198">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58d9e-198">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="58d9e-199">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="58d9e-199">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="58d9e-200">C#</span><span class="sxs-lookup"><span data-stu-id="58d9e-200">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58d9e-201">Javascript</span><span class="sxs-lookup"><span data-stu-id="58d9e-201">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="58d9e-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58d9e-202">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="58d9e-203">Confira também</span><span class="sxs-lookup"><span data-stu-id="58d9e-203">See also</span></span>

- [<span data-ttu-id="58d9e-204">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="58d9e-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="58d9e-205">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="58d9e-205">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="58d9e-206">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="58d9e-206">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

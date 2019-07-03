---
title: Criar grupo
description: Crie um novo grupo ou grupo de segurança do Office 365.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: cee571584f37feece435892caef0b0c648d13184
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440278"
---
# <a name="create-group"></a><span data-ttu-id="41aa6-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="41aa6-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41aa6-104">Crie um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41aa6-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="41aa6-105">Você pode criar um dos seguintes grupos:</span><span class="sxs-lookup"><span data-stu-id="41aa6-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="41aa6-106">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="41aa6-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="41aa6-107">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="41aa6-107">Security group</span></span>

<span data-ttu-id="41aa6-108">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="41aa6-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="41aa6-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="41aa6-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="41aa6-110">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="41aa6-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="41aa6-111">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="41aa6-111">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41aa6-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="41aa6-112">Permissions</span></span>
<span data-ttu-id="41aa6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41aa6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41aa6-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41aa6-115">Permission type</span></span>      | <span data-ttu-id="41aa6-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41aa6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41aa6-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41aa6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="41aa6-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41aa6-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="41aa6-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41aa6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41aa6-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41aa6-120">Not supported.</span></span>    |
|<span data-ttu-id="41aa6-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41aa6-121">Application</span></span> | <span data-ttu-id="41aa6-122">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41aa6-122">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41aa6-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41aa6-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="41aa6-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41aa6-124">Request headers</span></span>

| <span data-ttu-id="41aa6-125">Nome</span><span class="sxs-lookup"><span data-stu-id="41aa6-125">Name</span></span>       | <span data-ttu-id="41aa6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="41aa6-126">Type</span></span> | <span data-ttu-id="41aa6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="41aa6-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41aa6-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="41aa6-128">Authorization</span></span>  | <span data-ttu-id="41aa6-129">string</span><span class="sxs-lookup"><span data-stu-id="41aa6-129">string</span></span>  | <span data-ttu-id="41aa6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41aa6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41aa6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41aa6-132">Request body</span></span>

<span data-ttu-id="41aa6-133">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="41aa6-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="41aa6-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41aa6-134">Property</span></span> | <span data-ttu-id="41aa6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="41aa6-135">Type</span></span> | <span data-ttu-id="41aa6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="41aa6-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41aa6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="41aa6-137">displayName</span></span> | <span data-ttu-id="41aa6-138">string</span><span class="sxs-lookup"><span data-stu-id="41aa6-138">string</span></span> | <span data-ttu-id="41aa6-139">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="41aa6-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="41aa6-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41aa6-140">Required.</span></span> |
| <span data-ttu-id="41aa6-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="41aa6-141">mailEnabled</span></span> | <span data-ttu-id="41aa6-142">booliano</span><span class="sxs-lookup"><span data-stu-id="41aa6-142">boolean</span></span> | <span data-ttu-id="41aa6-143">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="41aa6-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="41aa6-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41aa6-144">Required.</span></span> |
| <span data-ttu-id="41aa6-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="41aa6-145">mailNickname</span></span> | <span data-ttu-id="41aa6-146">string</span><span class="sxs-lookup"><span data-stu-id="41aa6-146">string</span></span> | <span data-ttu-id="41aa6-147">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="41aa6-147">The mail alias for the group.</span></span> <span data-ttu-id="41aa6-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41aa6-148">Required.</span></span> |
| <span data-ttu-id="41aa6-149">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="41aa6-149">securityEnabled</span></span> | <span data-ttu-id="41aa6-150">booliano</span><span class="sxs-lookup"><span data-stu-id="41aa6-150">boolean</span></span> | <span data-ttu-id="41aa6-151">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="41aa6-151">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="41aa6-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41aa6-152">Required.</span></span> |
| <span data-ttu-id="41aa6-153">owners</span><span class="sxs-lookup"><span data-stu-id="41aa6-153">owners</span></span> | <span data-ttu-id="41aa6-154">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="41aa6-154">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="41aa6-155">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="41aa6-155">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="41aa6-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="41aa6-156">Optional.</span></span> |
| <span data-ttu-id="41aa6-157">membros</span><span class="sxs-lookup"><span data-stu-id="41aa6-157">members</span></span> | <span data-ttu-id="41aa6-158">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="41aa6-158">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="41aa6-159">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="41aa6-159">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="41aa6-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="41aa6-160">Optional.</span></span> |

> <span data-ttu-id="41aa6-161">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="41aa6-161">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="41aa6-162">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="41aa6-162">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="41aa6-163">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="41aa6-163">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="41aa6-164">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="41aa6-164">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="41aa6-p112">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="41aa6-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="41aa6-167">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="41aa6-167">groupTypes options</span></span>

<span data-ttu-id="41aa6-168">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrado abaixo:</span><span class="sxs-lookup"><span data-stu-id="41aa6-168">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="41aa6-169">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="41aa6-169">Type of group</span></span> | <span data-ttu-id="41aa6-170">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="41aa6-170">Assigned membership</span></span> | <span data-ttu-id="41aa6-171">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="41aa6-171">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="41aa6-172">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="41aa6-172">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="41aa6-173">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="41aa6-173">Dynamic</span></span> | <span data-ttu-id="41aa6-174">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="41aa6-174">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="41aa6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="41aa6-175">Response</span></span>

<span data-ttu-id="41aa6-176">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41aa6-176">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="41aa6-177">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="41aa6-177">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="41aa6-178">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41aa6-178">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="41aa6-179">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="41aa6-179">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="41aa6-180">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="41aa6-180">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="41aa6-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41aa6-181">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41aa6-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="41aa6-182">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="41aa6-183">C#</span><span class="sxs-lookup"><span data-stu-id="41aa6-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41aa6-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="41aa6-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41aa6-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41aa6-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41aa6-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="41aa6-186">Response</span></span>

<span data-ttu-id="41aa6-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41aa6-187">The following is an example of the response.</span></span>

><span data-ttu-id="41aa6-188">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41aa6-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41aa6-189">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41aa6-189">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="41aa6-190">Exemplo 2: Criando um grupo do Office 365 com um proprietário e membros</span><span class="sxs-lookup"><span data-stu-id="41aa6-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="41aa6-191">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="41aa6-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="41aa6-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41aa6-192">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41aa6-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="41aa6-193">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="41aa6-194">C#</span><span class="sxs-lookup"><span data-stu-id="41aa6-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41aa6-195">Javascript</span><span class="sxs-lookup"><span data-stu-id="41aa6-195">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41aa6-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41aa6-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41aa6-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="41aa6-197">Response</span></span> 

<span data-ttu-id="41aa6-198">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="41aa6-198">The following is an example of a successful response.</span></span> <span data-ttu-id="41aa6-199">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="41aa6-199">It includes only default properties.</span></span> <span data-ttu-id="41aa6-200">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="41aa6-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="41aa6-201">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41aa6-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41aa6-202">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41aa6-202">All the default properties are returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="41aa6-203">Confira também</span><span class="sxs-lookup"><span data-stu-id="41aa6-203">See also</span></span>

- [<span data-ttu-id="41aa6-204">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="41aa6-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="41aa6-205">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="41aa6-205">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="41aa6-206">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="41aa6-206">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->

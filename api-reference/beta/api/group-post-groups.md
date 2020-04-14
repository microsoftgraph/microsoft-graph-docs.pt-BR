---
title: Criar grupo
description: Crie um novo grupo ou grupo de segurança do Office 365.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e4fc80fc664404a0d17d535282e0d791b7e96cbb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396610"
---
# <a name="create-group"></a><span data-ttu-id="139b7-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="139b7-103">Create group</span></span>

<span data-ttu-id="139b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="139b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="139b7-105">Crie um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="139b7-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="139b7-106">Você pode criar um dos seguintes grupos:</span><span class="sxs-lookup"><span data-stu-id="139b7-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="139b7-107">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="139b7-107">Office 365 group (unified group)</span></span>
* <span data-ttu-id="139b7-108">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="139b7-108">Security group</span></span>

<span data-ttu-id="139b7-109">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="139b7-110">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="139b7-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="139b7-111">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="139b7-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="139b7-112">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="139b7-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="139b7-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="139b7-113">Permissions</span></span>
<span data-ttu-id="139b7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="139b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="139b7-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="139b7-116">Permission type</span></span>      | <span data-ttu-id="139b7-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="139b7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="139b7-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="139b7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="139b7-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="139b7-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="139b7-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="139b7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="139b7-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="139b7-121">Not supported.</span></span>    |
|<span data-ttu-id="139b7-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="139b7-122">Application</span></span> | <span data-ttu-id="139b7-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="139b7-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="139b7-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="139b7-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="139b7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="139b7-125">Request headers</span></span>

| <span data-ttu-id="139b7-126">Nome</span><span class="sxs-lookup"><span data-stu-id="139b7-126">Name</span></span>       | <span data-ttu-id="139b7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="139b7-127">Type</span></span> | <span data-ttu-id="139b7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="139b7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="139b7-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="139b7-129">Authorization</span></span>  | <span data-ttu-id="139b7-130">string</span><span class="sxs-lookup"><span data-stu-id="139b7-130">string</span></span>  | <span data-ttu-id="139b7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="139b7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="139b7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="139b7-133">Request body</span></span>

<span data-ttu-id="139b7-134">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="139b7-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="139b7-135">Property</span></span> | <span data-ttu-id="139b7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="139b7-136">Type</span></span> | <span data-ttu-id="139b7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="139b7-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="139b7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="139b7-138">displayName</span></span> | <span data-ttu-id="139b7-139">string</span><span class="sxs-lookup"><span data-stu-id="139b7-139">string</span></span> | <span data-ttu-id="139b7-140">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="139b7-141">Comprimento máximo: 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="139b7-141">Maximum length: 256 characters.</span></span> <span data-ttu-id="139b7-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="139b7-142">Required.</span></span> |
| <span data-ttu-id="139b7-143">description</span><span class="sxs-lookup"><span data-stu-id="139b7-143">description</span></span> | <span data-ttu-id="139b7-144">string</span><span class="sxs-lookup"><span data-stu-id="139b7-144">string</span></span> | <span data-ttu-id="139b7-145">Uma descrição para o grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-145">A description for the group.</span></span> <span data-ttu-id="139b7-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="139b7-146">Optional.</span></span> |
| <span data-ttu-id="139b7-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="139b7-147">mailEnabled</span></span> | <span data-ttu-id="139b7-148">booliano</span><span class="sxs-lookup"><span data-stu-id="139b7-148">boolean</span></span> | <span data-ttu-id="139b7-149">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="139b7-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="139b7-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="139b7-150">Required.</span></span> |
| <span data-ttu-id="139b7-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="139b7-151">mailNickname</span></span> | <span data-ttu-id="139b7-152">string</span><span class="sxs-lookup"><span data-stu-id="139b7-152">string</span></span> | <span data-ttu-id="139b7-153">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-153">The mail alias for the group.</span></span> <span data-ttu-id="139b7-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="139b7-154">Required.</span></span> |
| <span data-ttu-id="139b7-155">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="139b7-155">securityEnabled</span></span> | <span data-ttu-id="139b7-156">booliano</span><span class="sxs-lookup"><span data-stu-id="139b7-156">boolean</span></span> | <span data-ttu-id="139b7-157">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="139b7-157">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="139b7-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="139b7-158">Required.</span></span> |
| <span data-ttu-id="139b7-159">owners</span><span class="sxs-lookup"><span data-stu-id="139b7-159">owners</span></span> | <span data-ttu-id="139b7-160">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="139b7-160">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="139b7-161">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="139b7-161">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="139b7-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="139b7-162">Optional.</span></span> |
| <span data-ttu-id="139b7-163">membros</span><span class="sxs-lookup"><span data-stu-id="139b7-163">members</span></span> | <span data-ttu-id="139b7-164">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="139b7-164">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="139b7-165">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="139b7-165">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="139b7-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="139b7-166">Optional.</span></span> |
|<span data-ttu-id="139b7-167">visibility</span><span class="sxs-lookup"><span data-stu-id="139b7-167">visibility</span></span>|<span data-ttu-id="139b7-168">String</span><span class="sxs-lookup"><span data-stu-id="139b7-168">String</span></span>|<span data-ttu-id="139b7-169">Especifica a visibilidade de um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="139b7-169">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="139b7-170">Os valores possíveis são: `Private`, `Public`, `HiddenMembership` ou vazio (que é interpretado como `Public`).</span><span class="sxs-lookup"><span data-stu-id="139b7-170">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="139b7-171">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="139b7-171">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="139b7-172">Como o recurso de **grupo** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="139b7-172">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="139b7-173">**Observação:** Criar um grupo usando o Group. Criar a permissão de aplicativo sem especificar os proprietários criará o grupo anonimamente e o grupo não será modificado.</span><span class="sxs-lookup"><span data-stu-id="139b7-173">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="139b7-174">Você pode usar a operação `POST` e adicionar proprietários ao grupo enquanto a cria para especificar proprietários que podem modificar o grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-174">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="139b7-175">Criar um Grupo do Office 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="139b7-175">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="139b7-176">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="139b7-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="139b7-177">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-177">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="139b7-178">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="139b7-178">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="139b7-179">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="139b7-179">groupTypes options</span></span>

<span data-ttu-id="139b7-180">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrad.</span><span class="sxs-lookup"><span data-stu-id="139b7-180">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="139b7-181">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="139b7-181">Type of group</span></span> | <span data-ttu-id="139b7-182">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="139b7-182">Assigned membership</span></span> | <span data-ttu-id="139b7-183">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="139b7-183">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="139b7-184">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="139b7-184">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="139b7-185">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="139b7-185">Dynamic</span></span> | <span data-ttu-id="139b7-186">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="139b7-186">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="139b7-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="139b7-187">Response</span></span>

<span data-ttu-id="139b7-188">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="139b7-188">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="139b7-189">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-189">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="139b7-190">Exemplos</span><span class="sxs-lookup"><span data-stu-id="139b7-190">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="139b7-191">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="139b7-191">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="139b7-192">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="139b7-192">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="139b7-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="139b7-193">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="139b7-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="139b7-194">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="139b7-195">C#</span><span class="sxs-lookup"><span data-stu-id="139b7-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="139b7-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="139b7-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="139b7-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="139b7-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="139b7-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="139b7-198">Response</span></span>

<span data-ttu-id="139b7-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="139b7-199">The following is an example of the response.</span></span>

><span data-ttu-id="139b7-200">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="139b7-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="139b7-201">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="139b7-201">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="139b7-202">Exemplo 2: Criando um grupo do Office 365 com um proprietário e membros</span><span class="sxs-lookup"><span data-stu-id="139b7-202">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="139b7-203">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="139b7-203">The following example creates an Office 365 group with an owner and members specified.</span></span> <span data-ttu-id="139b7-204">Observe que, no máximo, 20 relações, como proprietários e membros, podem ser adicionadas como parte da criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="139b7-204">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="139b7-205">Posteriormente, você pode adicionar mais membros, usando a API [adicionar membro](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) ou o envio em lotes JSON.</span><span class="sxs-lookup"><span data-stu-id="139b7-205">You can subsequently add more members by using the [add member](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="139b7-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="139b7-206">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="139b7-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="139b7-207">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="139b7-208">C#</span><span class="sxs-lookup"><span data-stu-id="139b7-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="139b7-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="139b7-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="139b7-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="139b7-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="139b7-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="139b7-211">Response</span></span> 

<span data-ttu-id="139b7-212">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="139b7-212">The following is an example of a successful response.</span></span> <span data-ttu-id="139b7-213">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="139b7-213">It includes only default properties.</span></span> <span data-ttu-id="139b7-214">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="139b7-214">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="139b7-215">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="139b7-215">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="139b7-216">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="139b7-216">All the default properties are returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="139b7-217">Confira também</span><span class="sxs-lookup"><span data-stu-id="139b7-217">See also</span></span>

- [<span data-ttu-id="139b7-218">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="139b7-218">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="139b7-219">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="139b7-219">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="139b7-220">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="139b7-220">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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

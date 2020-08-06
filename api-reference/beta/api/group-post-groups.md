---
title: Criar grupo
description: Criar um novo grupo ou grupo de segurança do Microsoft 365.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b5a9ab85dbb39f9f4dfde783e687a90276708826
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566830"
---
# <a name="create-group"></a><span data-ttu-id="37a52-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="37a52-103">Create group</span></span>

<span data-ttu-id="37a52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a52-105">Crie um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a52-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="37a52-106">Você pode criar um dos seguintes grupos:</span><span class="sxs-lookup"><span data-stu-id="37a52-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="37a52-107">Grupo do Microsoft 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="37a52-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="37a52-108">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="37a52-108">Security group</span></span>

<span data-ttu-id="37a52-109">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="37a52-110">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="37a52-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="37a52-111">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="37a52-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="37a52-112">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="37a52-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37a52-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="37a52-113">Permissions</span></span>
<span data-ttu-id="37a52-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a52-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37a52-116">Permission type</span></span>      | <span data-ttu-id="37a52-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37a52-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37a52-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37a52-118">Delegated (work or school account)</span></span> | <span data-ttu-id="37a52-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37a52-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="37a52-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37a52-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a52-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a52-121">Not supported.</span></span>    |
|<span data-ttu-id="37a52-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37a52-122">Application</span></span> | <span data-ttu-id="37a52-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a52-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37a52-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37a52-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="37a52-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37a52-125">Request headers</span></span>

| <span data-ttu-id="37a52-126">Nome</span><span class="sxs-lookup"><span data-stu-id="37a52-126">Name</span></span>       | <span data-ttu-id="37a52-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a52-127">Type</span></span> | <span data-ttu-id="37a52-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a52-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="37a52-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="37a52-129">Authorization</span></span>  | <span data-ttu-id="37a52-130">string</span><span class="sxs-lookup"><span data-stu-id="37a52-130">string</span></span>  | <span data-ttu-id="37a52-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a52-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37a52-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37a52-133">Request body</span></span>

<span data-ttu-id="37a52-134">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="37a52-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37a52-135">Property</span></span> | <span data-ttu-id="37a52-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a52-136">Type</span></span> | <span data-ttu-id="37a52-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a52-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="37a52-138">displayName</span><span class="sxs-lookup"><span data-stu-id="37a52-138">displayName</span></span> | <span data-ttu-id="37a52-139">string</span><span class="sxs-lookup"><span data-stu-id="37a52-139">string</span></span> | <span data-ttu-id="37a52-140">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="37a52-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a52-141">Required.</span></span> |
| <span data-ttu-id="37a52-142">description</span><span class="sxs-lookup"><span data-stu-id="37a52-142">description</span></span> | <span data-ttu-id="37a52-143">string</span><span class="sxs-lookup"><span data-stu-id="37a52-143">string</span></span> | <span data-ttu-id="37a52-144">Uma descrição para o grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-144">A description for the group.</span></span> <span data-ttu-id="37a52-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a52-145">Optional.</span></span> |
| <span data-ttu-id="37a52-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="37a52-146">isAssignableToRole</span></span> | <span data-ttu-id="37a52-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="37a52-147">Boolean</span></span> | <span data-ttu-id="37a52-148">Definir para **true** para habilitar o grupo a ser atribuído uma função do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37a52-148">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="37a52-149">Somente o Administrador com Função Privilegiada e o Administrador Global podem definir o valor dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="37a52-149">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="37a52-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a52-150">Optional.</span></span> |
| <span data-ttu-id="37a52-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="37a52-151">mailEnabled</span></span> | <span data-ttu-id="37a52-152">booliano</span><span class="sxs-lookup"><span data-stu-id="37a52-152">boolean</span></span> | <span data-ttu-id="37a52-153">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="37a52-153">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="37a52-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a52-154">Required.</span></span> |
| <span data-ttu-id="37a52-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="37a52-155">mailNickname</span></span> | <span data-ttu-id="37a52-156">string</span><span class="sxs-lookup"><span data-stu-id="37a52-156">string</span></span> | <span data-ttu-id="37a52-157">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-157">The mail alias for the group.</span></span> <span data-ttu-id="37a52-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a52-158">Required.</span></span> |
| <span data-ttu-id="37a52-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="37a52-159">securityEnabled</span></span> | <span data-ttu-id="37a52-160">booliano</span><span class="sxs-lookup"><span data-stu-id="37a52-160">boolean</span></span> | <span data-ttu-id="37a52-161">Defina como **true** para grupos habilitados para segurança, incluindo grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="37a52-161">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="37a52-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a52-162">Required.</span></span> |
| <span data-ttu-id="37a52-163">owners</span><span class="sxs-lookup"><span data-stu-id="37a52-163">owners</span></span> | <span data-ttu-id="37a52-164">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="37a52-164">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="37a52-165">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="37a52-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="37a52-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a52-166">Optional.</span></span> |
| <span data-ttu-id="37a52-167">membros</span><span class="sxs-lookup"><span data-stu-id="37a52-167">members</span></span> | <span data-ttu-id="37a52-168">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="37a52-168">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="37a52-169">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="37a52-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="37a52-170">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37a52-170">Optional.</span></span> |
|<span data-ttu-id="37a52-171">visibility</span><span class="sxs-lookup"><span data-stu-id="37a52-171">visibility</span></span>|<span data-ttu-id="37a52-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37a52-172">String</span></span>|<span data-ttu-id="37a52-173">Especifica a visibilidade de um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="37a52-173">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="37a52-174">Os valores possíveis são: `Private`, `Public`, `HiddenMembership` ou vazio (que é interpretado como `Public`).</span><span class="sxs-lookup"><span data-stu-id="37a52-174">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="37a52-175">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="37a52-175">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="37a52-176">Como o recurso de **grupo** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="37a52-176">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="37a52-177">**Observação:** Criar um grupo usando o Group. Criar a permissão de aplicativo sem especificar os proprietários criará o grupo anonimamente e o grupo não será modificado.</span><span class="sxs-lookup"><span data-stu-id="37a52-177">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="37a52-178">Você pode usar a operação `POST` e adicionar proprietários ao grupo enquanto a cria para especificar proprietários que podem modificar o grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-178">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="37a52-179">Ao criar um grupo do Microsoft 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários, o grupo será criado anonimamente.</span><span class="sxs-lookup"><span data-stu-id="37a52-179">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="37a52-180">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="37a52-180">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="37a52-181">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-181">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="37a52-182">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="37a52-182">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="37a52-183">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="37a52-183">groupTypes options</span></span>

<span data-ttu-id="37a52-184">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrad.</span><span class="sxs-lookup"><span data-stu-id="37a52-184">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="37a52-185">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="37a52-185">Type of group</span></span> | <span data-ttu-id="37a52-186">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="37a52-186">Assigned membership</span></span> | <span data-ttu-id="37a52-187">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="37a52-187">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="37a52-188">Microsoft 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="37a52-188">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="37a52-189">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="37a52-189">Dynamic</span></span> | <span data-ttu-id="37a52-190">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="37a52-190">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="37a52-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a52-191">Response</span></span>

<span data-ttu-id="37a52-192">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37a52-192">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="37a52-193">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-193">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="37a52-194">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37a52-194">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="37a52-195">Exemplo 1: Criar um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="37a52-195">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="37a52-196">O exemplo a seguir cria um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="37a52-196">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="37a52-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a52-197">Request</span></span>

<span data-ttu-id="37a52-198">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a52-198">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37a52-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a52-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37a52-200">C#</span><span class="sxs-lookup"><span data-stu-id="37a52-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a52-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a52-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a52-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a52-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37a52-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a52-203">Response</span></span>

<span data-ttu-id="37a52-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37a52-204">The following is an example of the response.</span></span>

><span data-ttu-id="37a52-205">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37a52-205">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37a52-206">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37a52-206">All the default properties are returned from an actual call.</span></span>

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
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
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
   "isAssignableToRole": null,
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
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-microsoft-365-group-with-an-owner-and-members"></a><span data-ttu-id="37a52-207">Exemplo 2: Criar um grupo do Microsoft 365 com um proprietário e membros</span><span class="sxs-lookup"><span data-stu-id="37a52-207">Example 2: Create a Microsoft 365 group with an owner and members</span></span>

<span data-ttu-id="37a52-208">O exemplo a seguir cria um grupo do Microsoft 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="37a52-208">The following example creates a Microsoft 365 group with an owner and members specified.</span></span> <span data-ttu-id="37a52-209">Observe que, no máximo, 20 relações, como proprietários e membros, podem ser adicionadas como parte da criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="37a52-209">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="37a52-210">Posteriormente, você pode adicionar mais membros, usando a API [adicionar membro](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) ou o envio em lotes JSON.</span><span class="sxs-lookup"><span data-stu-id="37a52-210">You can subsequently add more members by using the [add member](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="37a52-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a52-211">Request</span></span>

<span data-ttu-id="37a52-212">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a52-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37a52-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a52-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37a52-214">C#</span><span class="sxs-lookup"><span data-stu-id="37a52-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a52-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a52-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a52-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a52-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37a52-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a52-217">Response</span></span> 

<span data-ttu-id="37a52-218">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="37a52-218">The following is an example of a successful response.</span></span> <span data-ttu-id="37a52-219">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="37a52-219">It includes only default properties.</span></span> <span data-ttu-id="37a52-220">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="37a52-220">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="37a52-221">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37a52-221">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37a52-222">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37a52-222">All the default properties are returned from an actual call.</span></span>

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
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "expirationDateTime": null,
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": null,
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
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
    "securityIdentifier": "S-1-12-1-1905728287-1207447622-870010782-555555555",
    "theme": null,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="37a52-223">Exemplo 3: Criar um grupo que pode ser atribuído a uma função do Azure AD</span><span class="sxs-lookup"><span data-stu-id="37a52-223">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="37a52-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a52-224">Request</span></span>

<span data-ttu-id="37a52-225">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a52-225">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37a52-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a52-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group assignable to a role",
  "displayName": "Role assignable group",
  "groupTypes": [
    "Unified"
  ],
  "isAssignableToRole": true,
  "mailEnabled": true,
  "securityEnabled": true,
  "mailNickname": "contosohelpdeskadministrators",
  "visibility" : "Private"
}
```
# <a name="c"></a>[<span data-ttu-id="37a52-227">C#</span><span class="sxs-lookup"><span data-stu-id="37a52-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a52-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a52-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a52-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a52-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="37a52-230">**Observação:** As propriedades de **visibilidade** e **groupTypes** não são necessárias para a criação, mas são preenchidas automaticamente com esses valores.</span><span class="sxs-lookup"><span data-stu-id="37a52-230">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="37a52-231">Um grupo com a propriedade **isAssignableToRole** definida como `true` não pode ser do tipo associação dinâmica.</span><span class="sxs-lookup"><span data-stu-id="37a52-231">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="37a52-232">Para mais informações, consulte [Usando um grupo para gerenciar as atribuições de funções do Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="37a52-232">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="37a52-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a52-233">Response</span></span>

<span data-ttu-id="37a52-234">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37a52-234">The following is an example of the response.</span></span> <span data-ttu-id="37a52-235">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="37a52-235">It includes only default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_role_enabled_group"
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
  "description": "Group assignable to a role",
  "displayName": "Role assignable group",
  "expirationDateTime": null,
  "groupTypes": [
    "Unified"
  ],
  "isAssignableToRole": true,
  "mail": "operations2019@contoso.com",
  "mailEnabled": true,
  "mailNickname": "contosohelpdeskadministrators",
  "membershipRule": null,
  "membershipRuleProcessingState": null,
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
  "securityEnabled": true,
  "securityIdentifier": "S-1-12-1-1905728287-1207447622-870010782-555555555",
  "theme": null,
  "visibility": "Private",
  "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="37a52-236">Confira também</span><span class="sxs-lookup"><span data-stu-id="37a52-236">See also</span></span>

- [<span data-ttu-id="37a52-237">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="37a52-237">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="37a52-238">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="37a52-238">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="37a52-239">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="37a52-239">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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

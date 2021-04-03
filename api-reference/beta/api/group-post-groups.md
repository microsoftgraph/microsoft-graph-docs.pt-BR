---
title: Criar grupo
description: Criar um novo grupo ou grupo de segurança do Microsoft 365.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 871d990342807a9742ce9125c62e730fec39cd10
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507942"
---
# <a name="create-group"></a><span data-ttu-id="c4430-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="c4430-103">Create group</span></span>

<span data-ttu-id="c4430-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4430-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4430-105">Crie um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4430-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="c4430-106">Você pode criar um dos seguintes grupos:</span><span class="sxs-lookup"><span data-stu-id="c4430-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="c4430-107">Grupo do Microsoft 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="c4430-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="c4430-108">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="c4430-108">Security group</span></span>

<span data-ttu-id="c4430-109">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="c4430-110">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="c4430-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="c4430-111">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="c4430-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="c4430-112">**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="c4430-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4430-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4430-113">Permissions</span></span>
<span data-ttu-id="c4430-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4430-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4430-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4430-116">Permission type</span></span>      | <span data-ttu-id="c4430-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4430-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4430-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4430-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c4430-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4430-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="c4430-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4430-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4430-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4430-121">Not supported.</span></span>    |
|<span data-ttu-id="c4430-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4430-122">Application</span></span> | <span data-ttu-id="c4430-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4430-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4430-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4430-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="c4430-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4430-125">Request headers</span></span>

| <span data-ttu-id="c4430-126">Nome</span><span class="sxs-lookup"><span data-stu-id="c4430-126">Name</span></span>       | <span data-ttu-id="c4430-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4430-127">Type</span></span> | <span data-ttu-id="c4430-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4430-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4430-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4430-129">Authorization</span></span>  | <span data-ttu-id="c4430-130">string</span><span class="sxs-lookup"><span data-stu-id="c4430-130">string</span></span>  | <span data-ttu-id="c4430-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4430-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4430-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4430-133">Request body</span></span>

<span data-ttu-id="c4430-134">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="c4430-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4430-135">Property</span></span> | <span data-ttu-id="c4430-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4430-136">Type</span></span> | <span data-ttu-id="c4430-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4430-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4430-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c4430-138">displayName</span></span> | <span data-ttu-id="c4430-139">string</span><span class="sxs-lookup"><span data-stu-id="c4430-139">string</span></span> | <span data-ttu-id="c4430-140">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="c4430-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4430-141">Required.</span></span> |
| <span data-ttu-id="c4430-142">description</span><span class="sxs-lookup"><span data-stu-id="c4430-142">description</span></span> | <span data-ttu-id="c4430-143">string</span><span class="sxs-lookup"><span data-stu-id="c4430-143">string</span></span> | <span data-ttu-id="c4430-144">Uma descrição para o grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-144">A description for the group.</span></span> <span data-ttu-id="c4430-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c4430-145">Optional.</span></span> |
| <span data-ttu-id="c4430-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="c4430-146">isAssignableToRole</span></span> | <span data-ttu-id="c4430-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4430-147">Boolean</span></span> | <span data-ttu-id="c4430-148">Definir para **true** para habilitar o grupo a ser atribuído uma função do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c4430-148">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="c4430-149">Somente o Administrador com Função Privilegiada e o Administrador Global podem definir o valor dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="c4430-149">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="c4430-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c4430-150">Optional.</span></span> |
| <span data-ttu-id="c4430-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="c4430-151">mailEnabled</span></span> | <span data-ttu-id="c4430-152">booliano</span><span class="sxs-lookup"><span data-stu-id="c4430-152">boolean</span></span> | <span data-ttu-id="c4430-153">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="c4430-153">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="c4430-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4430-154">Required.</span></span> |
| <span data-ttu-id="c4430-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c4430-155">mailNickname</span></span> | <span data-ttu-id="c4430-156">string</span><span class="sxs-lookup"><span data-stu-id="c4430-156">string</span></span> | <span data-ttu-id="c4430-157">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-157">The mail alias for the group.</span></span> <span data-ttu-id="c4430-158">Esses caracteres não podem ser usados no mailNickName: `@()\[]";:.<>,SPACE`.</span><span class="sxs-lookup"><span data-stu-id="c4430-158">These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`.</span></span> <span data-ttu-id="c4430-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4430-159">Required.</span></span> |
| <span data-ttu-id="c4430-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="c4430-160">securityEnabled</span></span> | <span data-ttu-id="c4430-161">booliano</span><span class="sxs-lookup"><span data-stu-id="c4430-161">boolean</span></span> | <span data-ttu-id="c4430-162">Defina como **true** para grupos habilitados para segurança, incluindo grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4430-162">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="c4430-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4430-163">Required.</span></span> |
| <span data-ttu-id="c4430-164">owners</span><span class="sxs-lookup"><span data-stu-id="c4430-164">owners</span></span> | <span data-ttu-id="c4430-165">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c4430-165">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="c4430-166">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="c4430-166">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="c4430-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c4430-167">Optional.</span></span> |
| <span data-ttu-id="c4430-168">membros</span><span class="sxs-lookup"><span data-stu-id="c4430-168">members</span></span> | <span data-ttu-id="c4430-169">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c4430-169">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="c4430-170">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="c4430-170">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="c4430-171">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c4430-171">Optional.</span></span> |
|<span data-ttu-id="c4430-172">visibility</span><span class="sxs-lookup"><span data-stu-id="c4430-172">visibility</span></span>|<span data-ttu-id="c4430-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4430-173">String</span></span>|<span data-ttu-id="c4430-174">Especifica a visibilidade de um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4430-174">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="c4430-175">Os valores possíveis são: `Private`, `Public`, `HiddenMembership` ou vazio (que é interpretado como `Public`).</span><span class="sxs-lookup"><span data-stu-id="c4430-175">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="c4430-176">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="c4430-176">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="c4430-177">Como o recurso de **grupo** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="c4430-177">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="c4430-178">**Observação:** Criar um grupo usando o Group. Criar a permissão de aplicativo sem especificar os proprietários criará o grupo anonimamente e o grupo não será modificado.</span><span class="sxs-lookup"><span data-stu-id="c4430-178">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="c4430-179">Você pode usar a operação `POST` e adicionar proprietários ao grupo enquanto a cria para especificar proprietários que podem modificar o grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-179">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="c4430-180">Ao criar um grupo do Microsoft 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários, o grupo será criado anonimamente.</span><span class="sxs-lookup"><span data-stu-id="c4430-180">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="c4430-181">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="c4430-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="c4430-182">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-182">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="c4430-183">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="c4430-183">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="c4430-184">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="c4430-184">groupTypes options</span></span>

<span data-ttu-id="c4430-185">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrad.</span><span class="sxs-lookup"><span data-stu-id="c4430-185">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="c4430-186">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="c4430-186">Type of group</span></span> | <span data-ttu-id="c4430-187">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="c4430-187">Assigned membership</span></span> | <span data-ttu-id="c4430-188">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="c4430-188">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="c4430-189">Microsoft 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="c4430-189">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="c4430-190">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="c4430-190">Dynamic</span></span> | <span data-ttu-id="c4430-191">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="c4430-191">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="c4430-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4430-192">Response</span></span>

<span data-ttu-id="c4430-193">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4430-193">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="c4430-194">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-194">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="c4430-195">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4430-195">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="c4430-196">Exemplo 1: Criar um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c4430-196">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="c4430-197">O exemplo a seguir cria um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4430-197">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="c4430-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4430-198">Request</span></span>

<span data-ttu-id="c4430-199">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4430-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4430-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4430-200">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4430-201">C#</span><span class="sxs-lookup"><span data-stu-id="c4430-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4430-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4430-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4430-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4430-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4430-204">Java</span><span class="sxs-lookup"><span data-stu-id="c4430-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4430-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4430-205">Response</span></span>

<span data-ttu-id="c4430-206">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4430-206">The following is an example of the response.</span></span>

><span data-ttu-id="c4430-207">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4430-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4430-208">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4430-208">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-a-security-group-with-an-owner-and-members"></a><span data-ttu-id="c4430-209">Exemplo 2: criar um grupo de segurança com um proprietário e membros</span><span class="sxs-lookup"><span data-stu-id="c4430-209">Example 2: Create a security group with an owner and members</span></span>

<span data-ttu-id="c4430-210">O exemplo a seguir cria um grupo de segurança com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="c4430-210">The following example creates a security group with an owner and members specified.</span></span> <span data-ttu-id="c4430-211">Observe que, no máximo, 20 relações, como proprietários e membros, podem ser adicionadas como parte da criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="c4430-211">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="c4430-212">Posteriormente, você pode adicionar mais membros, usando a API [adicionar membro](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) ou o envio em lotes JSON.</span><span class="sxs-lookup"><span data-stu-id="c4430-212">You can subsequently add more members by using the [add member](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="c4430-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4430-213">Request</span></span>

<span data-ttu-id="c4430-214">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4430-214">The following is an example of the request.</span></span>

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
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="c4430-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4430-215">Response</span></span> 

<span data-ttu-id="c4430-216">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c4430-216">The following is an example of a successful response.</span></span> <span data-ttu-id="c4430-217">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="c4430-217">It includes only default properties.</span></span> <span data-ttu-id="c4430-218">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="c4430-218">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="c4430-219">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4430-219">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4430-220">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4430-220">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="c4430-221">Exemplo 3: Criar um grupo que pode ser atribuído a uma função do Azure AD</span><span class="sxs-lookup"><span data-stu-id="c4430-221">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="c4430-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4430-222">Request</span></span>

<span data-ttu-id="c4430-223">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4430-223">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c4430-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4430-224">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4430-225">C#</span><span class="sxs-lookup"><span data-stu-id="c4430-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4430-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4430-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4430-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4430-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4430-228">Java</span><span class="sxs-lookup"><span data-stu-id="c4430-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="c4430-229">**Observação:** As propriedades de **visibilidade** e **groupTypes** não são necessárias para a criação, mas são preenchidas automaticamente com esses valores.</span><span class="sxs-lookup"><span data-stu-id="c4430-229">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="c4430-230">Um grupo com a propriedade **isAssignableToRole** definida como `true` não pode ser do tipo associação dinâmica.</span><span class="sxs-lookup"><span data-stu-id="c4430-230">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="c4430-231">Para mais informações, consulte [Usando um grupo para gerenciar as atribuições de funções do Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="c4430-231">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="c4430-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4430-232">Response</span></span>

<span data-ttu-id="c4430-233">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4430-233">The following is an example of the response.</span></span> <span data-ttu-id="c4430-234">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="c4430-234">It includes only default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c4430-235">Confira também</span><span class="sxs-lookup"><span data-stu-id="c4430-235">See also</span></span>

- [<span data-ttu-id="c4430-236">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c4430-236">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c4430-237">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c4430-237">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c4430-238">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="c4430-238">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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



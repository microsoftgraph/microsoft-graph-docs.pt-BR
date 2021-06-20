---
title: Criar grupo
description: 'Crie um novo grupo conforme especificado no corpo da solicitação. '
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e58f8f9bbd87d73c4072936ce69089268fd9ca6
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030884"
---
# <a name="create-group"></a><span data-ttu-id="9a0e4-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="9a0e4-103">Create group</span></span>

<span data-ttu-id="9a0e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a0e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a0e4-p101">Crie um novo grupo conforme especificado no corpo da solicitação. Você pode criar os seguintes tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p101">Create a new group as specified in the request body. You can create the following types of groups:</span></span>

* <span data-ttu-id="9a0e4-107">Grupo do Microsoft 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="9a0e4-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="9a0e4-108">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="9a0e4-108">Security group</span></span>

<span data-ttu-id="9a0e4-109">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="9a0e4-110">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="9a0e4-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="9a0e4-111">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="9a0e4-112">**Observação**: Embora o Microsoft Teams tenha como base grupos do Microsoft 365, atualmente não é possível criar uma equipe por meio desta API.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-112">**Note**: Although Microsoft Teams is built on Microsoft 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="9a0e4-113">Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-113">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a0e4-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a0e4-114">Permissions</span></span>
<span data-ttu-id="9a0e4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a0e4-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a0e4-117">Permission type</span></span>      | <span data-ttu-id="9a0e4-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a0e4-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a0e4-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a0e4-119">Delegated (work or school account)</span></span> | <span data-ttu-id="9a0e4-120">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a0e4-120">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="9a0e4-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a0e4-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a0e4-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-122">Not supported.</span></span>    |
|<span data-ttu-id="9a0e4-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a0e4-123">Application</span></span> | <span data-ttu-id="9a0e4-124">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0e4-124">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a0e4-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0e4-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="9a0e4-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e4-126">Request headers</span></span>
| <span data-ttu-id="9a0e4-127">Nome</span><span class="sxs-lookup"><span data-stu-id="9a0e4-127">Name</span></span>       | <span data-ttu-id="9a0e4-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a0e4-128">Type</span></span> | <span data-ttu-id="9a0e4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a0e4-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a0e4-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a0e4-130">Authorization</span></span>  | <span data-ttu-id="9a0e4-131">string</span><span class="sxs-lookup"><span data-stu-id="9a0e4-131">string</span></span>  | <span data-ttu-id="9a0e4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a0e4-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a0e4-134">Content-Type</span></span>  | <span data-ttu-id="9a0e4-135">application/json</span><span class="sxs-lookup"><span data-stu-id="9a0e4-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a0e4-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e4-136">Request body</span></span>
<span data-ttu-id="9a0e4-137">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="9a0e4-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a0e4-138">Property</span></span> | <span data-ttu-id="9a0e4-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a0e4-139">Type</span></span> | <span data-ttu-id="9a0e4-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a0e4-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a0e4-141">displayName</span><span class="sxs-lookup"><span data-stu-id="9a0e4-141">displayName</span></span> | <span data-ttu-id="9a0e4-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a0e4-142">string</span></span> | <span data-ttu-id="9a0e4-p106">O nome a ser exibido no livro de endereços do grupo. Comprimento máximo: 256 caracteres. Necessário.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p106">The name to display in the address book for the group. Maximum length: 256 characters. Required.</span></span> |
| <span data-ttu-id="9a0e4-146">description</span><span class="sxs-lookup"><span data-stu-id="9a0e4-146">description</span></span> | <span data-ttu-id="9a0e4-147">string</span><span class="sxs-lookup"><span data-stu-id="9a0e4-147">string</span></span> | <span data-ttu-id="9a0e4-148">Uma descrição para o grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-148">A description for the group.</span></span> <span data-ttu-id="9a0e4-149">Máx.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-149">Max.</span></span> <span data-ttu-id="9a0e4-150">comprimento: 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-150">length: 1024 characters.</span></span> <span data-ttu-id="9a0e4-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-151">Optional.</span></span> |
| <span data-ttu-id="9a0e4-152">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="9a0e4-152">isAssignableToRole</span></span> | <span data-ttu-id="9a0e4-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e4-153">Boolean</span></span> | <span data-ttu-id="9a0e4-154">Definir para **true** para habilitar o grupo a ser atribuído uma função do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-154">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="9a0e4-155">Somente o Administrador com Função Privilegiada e o Administrador Global podem definir o valor dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-155">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="9a0e4-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-156">Optional.</span></span> |
| <span data-ttu-id="9a0e4-157">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="9a0e4-157">mailEnabled</span></span> | <span data-ttu-id="9a0e4-158">booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e4-158">boolean</span></span> | <span data-ttu-id="9a0e4-159">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-159">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="9a0e4-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-160">Required.</span></span> |
| <span data-ttu-id="9a0e4-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9a0e4-161">mailNickname</span></span> | <span data-ttu-id="9a0e4-162">string</span><span class="sxs-lookup"><span data-stu-id="9a0e4-162">string</span></span> | <span data-ttu-id="9a0e4-163">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-163">The mail alias for the group.</span></span> <span data-ttu-id="9a0e4-164">Máx.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-164">Max.</span></span> <span data-ttu-id="9a0e4-165">comprimento: 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-165">length: 64 characters.</span></span> <span data-ttu-id="9a0e4-166">Esses caracteres não podem ser usados no mailNickName: `@()\[]";:.<>,SPACE`.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-166">These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`.</span></span> <span data-ttu-id="9a0e4-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-167">Required.</span></span> |
| <span data-ttu-id="9a0e4-168">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="9a0e4-168">securityEnabled</span></span> | <span data-ttu-id="9a0e4-169">booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e4-169">boolean</span></span> | <span data-ttu-id="9a0e4-170">Defina como **true** para grupos habilitados para segurança, incluindo grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-170">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="9a0e4-171">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-171">Required.</span></span> |
| <span data-ttu-id="9a0e4-172">owners</span><span class="sxs-lookup"><span data-stu-id="9a0e4-172">owners</span></span> | <span data-ttu-id="9a0e4-173">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a0e4-173">string collection</span></span> | <span data-ttu-id="9a0e4-p112">Esta propriedade representa os proprietários do grupo na hora de criação. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p112">This property represents the owners for the group at creation time. Optional.</span></span> |
| <span data-ttu-id="9a0e4-176">membros</span><span class="sxs-lookup"><span data-stu-id="9a0e4-176">members</span></span> | <span data-ttu-id="9a0e4-177">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a0e4-177">string collection</span></span> | <span data-ttu-id="9a0e4-p113">Esta propriedade representa os membros do grupo na hora de criação. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p113">This property represents the members for the group at creation time. Optional.</span></span> |
|<span data-ttu-id="9a0e4-180">visibility</span><span class="sxs-lookup"><span data-stu-id="9a0e4-180">visibility</span></span>|<span data-ttu-id="9a0e4-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a0e4-181">String</span></span>|<span data-ttu-id="9a0e4-182">Especifica a visibilidade de um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-182">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="9a0e4-183">Os valores possíveis são: `Private`, `Public`, `HiddenMembership` ou vazio (que é interpretado como `Public`).</span><span class="sxs-lookup"><span data-stu-id="9a0e4-183">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="9a0e4-184">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-184">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="9a0e4-p115">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="9a0e4-187">**Observação:** Criar um grupo usando o Group. Criar a permissão de aplicativo sem especificar os proprietários criará o grupo anonimamente e o grupo não será modificado.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-187">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="9a0e4-188">Você pode usar a operação `POST` e adicionar proprietários ao grupo enquanto a cria para especificar proprietários que podem modificar o grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-188">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="9a0e4-189">Ao criar um grupo do Microsoft 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários, o grupo será criado anonimamente.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-189">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="9a0e4-190">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-190">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="9a0e4-191">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="9a0e4-191">groupTypes options</span></span>

<span data-ttu-id="9a0e4-192">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrad.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-192">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="9a0e4-193">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="9a0e4-193">Type of group</span></span> | <span data-ttu-id="9a0e4-194">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="9a0e4-194">Assigned membership</span></span> | <span data-ttu-id="9a0e4-195">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="9a0e4-195">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="9a0e4-196">Microsoft 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="9a0e4-196">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="9a0e4-197">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="9a0e4-197">Dynamic</span></span> | <span data-ttu-id="9a0e4-198">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="9a0e4-198">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="9a0e4-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0e4-199">Response</span></span>
<span data-ttu-id="9a0e4-200">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-200">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="9a0e4-201">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-201">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="9a0e4-202">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a0e4-202">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="9a0e4-203">Exemplo 1: Criar um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9a0e4-203">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="9a0e4-204">O exemplo a seguir cria um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-204">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="9a0e4-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e4-205">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9a0e4-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0e4-206">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9a0e4-207">C#</span><span class="sxs-lookup"><span data-stu-id="9a0e4-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a0e4-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a0e4-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a0e4-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a0e4-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a0e4-210">Java</span><span class="sxs-lookup"><span data-stu-id="9a0e4-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a0e4-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0e4-211">Response</span></span>

<span data-ttu-id="9a0e4-212">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-212">The following is an example of the response.</span></span>

><span data-ttu-id="9a0e4-213">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-213">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="9a0e4-214">Exemplo 2: criando um grupo com membros e proprietários</span><span class="sxs-lookup"><span data-stu-id="9a0e4-214">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="9a0e4-215">O exemplo a seguir cria um Grupo de segurança com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-215">The following example creates a Security group with an owner and members specified.</span></span> <span data-ttu-id="9a0e4-216">Observe que, no máximo, 20 relações, como proprietários e membros, podem ser adicionadas como parte da criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-216">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="9a0e4-217">Posteriormente, você pode adicionar mais membros, usando a API [adicionar membro](group-post-members.md) ou o envio em lotes JSON.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-217">You can subsequently add more members by using the [add member](group-post-members.md) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="9a0e4-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e4-218">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9a0e4-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0e4-219">HTTP</span></span>](#tab/http)
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
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9a0e4-220">C#</span><span class="sxs-lookup"><span data-stu-id="9a0e4-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a0e4-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a0e4-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a0e4-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a0e4-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a0e4-223">Java</span><span class="sxs-lookup"><span data-stu-id="9a0e4-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a0e4-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0e4-224">Response</span></span>

<span data-ttu-id="9a0e4-225">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-225">The following is an example of a successful response.</span></span> <span data-ttu-id="9a0e4-226">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-226">It includes only default properties.</span></span> <span data-ttu-id="9a0e4-227">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-227">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="9a0e4-228">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-228">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="9a0e4-229">Exemplo 3: Criar um grupo que pode ser atribuído a uma função do Azure AD</span><span class="sxs-lookup"><span data-stu-id="9a0e4-229">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="9a0e4-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e4-230">Request</span></span>

<span data-ttu-id="9a0e4-231">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups
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

> <span data-ttu-id="9a0e4-232">**Observação:** As propriedades de **visibilidade** e **groupTypes** não são necessárias para a criação, mas são preenchidas automaticamente com esses valores.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-232">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="9a0e4-233">Um grupo com a propriedade **isAssignableToRole** definida como `true` não pode ser do tipo de associação dinâmica e não pode ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-233">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type and cannot have an owner.</span></span> <span data-ttu-id="9a0e4-234">Para mais informações, consulte [Usando um grupo para gerenciar as atribuições de funções do Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="9a0e4-234">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="9a0e4-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0e4-235">Response</span></span>

<span data-ttu-id="9a0e4-p122">Veja a seguir o exemplo de uma resposta. Ela inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="9a0e4-p122">The following is an example of the response. It includes only default properties.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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
} -->


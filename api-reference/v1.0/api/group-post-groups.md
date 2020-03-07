---
title: Criar grupo
description: 'Crie um novo grupo conforme especificado no corpo da solicitação. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 418c24dcb3779725cadb41e59c712c870d1bd74a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516988"
---
# <a name="create-group"></a><span data-ttu-id="b6739-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="b6739-103">Create group</span></span>

<span data-ttu-id="b6739-104">Namespace: microsoft.graph Crie um novo grupo conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6739-104">Namespace: microsoft.graph Create a new group as specified in the request body.</span></span> <span data-ttu-id="b6739-105">Você pode criar os seguintes tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="b6739-105">You can create the following types of groups:</span></span>

* <span data-ttu-id="b6739-106">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="b6739-106">Office 365 group (unified group)</span></span>
* <span data-ttu-id="b6739-107">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="b6739-107">Security group</span></span>

<span data-ttu-id="b6739-108">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="b6739-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="b6739-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="b6739-110">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta do `$select` OData.</span><span class="sxs-lookup"><span data-stu-id="b6739-110">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="b6739-111">**Observação**: Embora o Microsoft Teams tenha como base grupos do Office 365, atualmente não é possível criar uma equipe por meio desta API.</span><span class="sxs-lookup"><span data-stu-id="b6739-111">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="b6739-112">Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b6739-112">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6739-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6739-113">Permissions</span></span>
<span data-ttu-id="b6739-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6739-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6739-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6739-116">Permission type</span></span>      | <span data-ttu-id="b6739-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6739-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6739-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6739-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b6739-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6739-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="b6739-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6739-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6739-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6739-121">Not supported.</span></span>    |
|<span data-ttu-id="b6739-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6739-122">Application</span></span> | <span data-ttu-id="b6739-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6739-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6739-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6739-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="b6739-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-125">Request headers</span></span>
| <span data-ttu-id="b6739-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b6739-126">Name</span></span>       | <span data-ttu-id="b6739-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6739-127">Type</span></span> | <span data-ttu-id="b6739-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6739-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6739-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6739-129">Authorization</span></span>  | <span data-ttu-id="b6739-130">string</span><span class="sxs-lookup"><span data-stu-id="b6739-130">string</span></span>  | <span data-ttu-id="b6739-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6739-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6739-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6739-133">Content-Type</span></span>  | <span data-ttu-id="b6739-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b6739-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6739-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-135">Request body</span></span>
<span data-ttu-id="b6739-136">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="b6739-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6739-137">Property</span></span> | <span data-ttu-id="b6739-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6739-138">Type</span></span> | <span data-ttu-id="b6739-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6739-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6739-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b6739-140">displayName</span></span> | <span data-ttu-id="b6739-141">string</span><span class="sxs-lookup"><span data-stu-id="b6739-141">string</span></span> | <span data-ttu-id="b6739-142">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="b6739-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6739-143">Required.</span></span> |
| <span data-ttu-id="b6739-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="b6739-144">mailEnabled</span></span> | <span data-ttu-id="b6739-145">booliano</span><span class="sxs-lookup"><span data-stu-id="b6739-145">boolean</span></span> | <span data-ttu-id="b6739-146">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="b6739-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="b6739-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6739-147">Required.</span></span> |
| <span data-ttu-id="b6739-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b6739-148">mailNickname</span></span> | <span data-ttu-id="b6739-149">string</span><span class="sxs-lookup"><span data-stu-id="b6739-149">string</span></span> | <span data-ttu-id="b6739-150">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-150">The mail alias for the group.</span></span> <span data-ttu-id="b6739-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6739-151">Required.</span></span> |
| <span data-ttu-id="b6739-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="b6739-152">securityEnabled</span></span> | <span data-ttu-id="b6739-153">booliano</span><span class="sxs-lookup"><span data-stu-id="b6739-153">boolean</span></span> | <span data-ttu-id="b6739-154">Defina como **verdadeiro** para grupos ativados por segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b6739-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="b6739-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6739-155">Required.</span></span> |
| <span data-ttu-id="b6739-156">owners</span><span class="sxs-lookup"><span data-stu-id="b6739-156">owners</span></span> | <span data-ttu-id="b6739-157">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6739-157">string collection</span></span> | <span data-ttu-id="b6739-158">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="b6739-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="b6739-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6739-159">Optional.</span></span> |
| <span data-ttu-id="b6739-160">membros</span><span class="sxs-lookup"><span data-stu-id="b6739-160">members</span></span> | <span data-ttu-id="b6739-161">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6739-161">string collection</span></span> | <span data-ttu-id="b6739-162">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="b6739-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="b6739-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6739-163">Optional.</span></span> |

> <span data-ttu-id="b6739-164">**Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.</span><span class="sxs-lookup"><span data-stu-id="b6739-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="b6739-165">Especifique outras propriedades graváveis conforme necessário para o seu grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="b6739-166">Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="b6739-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="b6739-167">**Observação:** Criar um grupo usando o Group. Criar a permissão de aplicativo sem especificar os proprietários criará o grupo anonimamente e o grupo não será modificado.</span><span class="sxs-lookup"><span data-stu-id="b6739-167">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="b6739-168">Você pode usar a operação `POST` e adicionar proprietários ao grupo enquanto a cria para especificar proprietários que podem modificar o grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-168">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="b6739-169">Criar um Grupo do Office 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="b6739-169">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="b6739-170">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="b6739-170">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="b6739-171">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="b6739-171">groupTypes options</span></span>

<span data-ttu-id="b6739-172">Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrad.</span><span class="sxs-lookup"><span data-stu-id="b6739-172">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="b6739-173">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="b6739-173">Type of group</span></span> | <span data-ttu-id="b6739-174">Associação atribuída</span><span class="sxs-lookup"><span data-stu-id="b6739-174">Assigned membership</span></span> | <span data-ttu-id="b6739-175">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="b6739-175">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="b6739-176">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="b6739-176">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="b6739-177">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="b6739-177">Dynamic</span></span> | <span data-ttu-id="b6739-178">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="b6739-178">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="b6739-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6739-179">Response</span></span>
<span data-ttu-id="b6739-180">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6739-180">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="b6739-181">A resposta inclui somente as propriedades padrão do grupo.</span><span class="sxs-lookup"><span data-stu-id="b6739-181">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="b6739-182">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6739-182">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="b6739-183">Exemplo 1: criando um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="b6739-183">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="b6739-184">O exemplo a seguir cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b6739-184">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="b6739-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-185">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b6739-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6739-186">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b6739-187">C#</span><span class="sxs-lookup"><span data-stu-id="b6739-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6739-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6739-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6739-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6739-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6739-190">Java</span><span class="sxs-lookup"><span data-stu-id="b6739-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6739-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6739-191">Response</span></span>

<span data-ttu-id="b6739-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6739-192">The following is an example of the response.</span></span>

><span data-ttu-id="b6739-193">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6739-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6739-194">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6739-194">All the default properties are returned from an actual call.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="b6739-195">Exemplo 2: criando um grupo com membros e proprietários</span><span class="sxs-lookup"><span data-stu-id="b6739-195">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="b6739-196">O exemplo a seguir cria um grupo do Office 365 com um proprietário e membros especificados.</span><span class="sxs-lookup"><span data-stu-id="b6739-196">The following example creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="b6739-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-197">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b6739-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6739-198">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b6739-199">C#</span><span class="sxs-lookup"><span data-stu-id="b6739-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6739-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6739-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6739-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6739-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6739-202">Java</span><span class="sxs-lookup"><span data-stu-id="b6739-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6739-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6739-203">Response</span></span>

<span data-ttu-id="b6739-204">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="b6739-204">The following is an example of a successful response.</span></span> <span data-ttu-id="b6739-205">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="b6739-205">It includes only default properties.</span></span> <span data-ttu-id="b6739-206">Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros.</span><span class="sxs-lookup"><span data-stu-id="b6739-206">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="b6739-207">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6739-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6739-208">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6739-208">All the default properties are returned from an actual call.</span></span>

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

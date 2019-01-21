---
title: Criar grupo
description: 'Use esta API para criar um novo grupo, conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: d0c02dfe2eba9488848cefb7f85241a2c40210e4
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726578"
---
# <a name="create-group"></a><span data-ttu-id="8c92d-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="8c92d-104">Create group</span></span>
<span data-ttu-id="8c92d-p102">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="8c92d-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="8c92d-107">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="8c92d-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="8c92d-108">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="8c92d-108">Dynamic group</span></span>
* <span data-ttu-id="8c92d-109">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="8c92d-109">Security group</span></span>

<span data-ttu-id="8c92d-110">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="8c92d-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="8c92d-111">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="8c92d-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="8c92d-112">Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="8c92d-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="8c92d-113">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="8c92d-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="8c92d-p105">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8c92d-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c92d-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c92d-116">Permissions</span></span>
<span data-ttu-id="8c92d-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c92d-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c92d-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c92d-119">Permission type</span></span>      | <span data-ttu-id="8c92d-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c92d-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c92d-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c92d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8c92d-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c92d-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c92d-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c92d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c92d-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c92d-124">Not supported.</span></span>    |
|<span data-ttu-id="8c92d-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c92d-125">Application</span></span> | <span data-ttu-id="8c92d-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c92d-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c92d-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c92d-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="8c92d-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c92d-128">Request headers</span></span>
| <span data-ttu-id="8c92d-129">Nome</span><span class="sxs-lookup"><span data-stu-id="8c92d-129">Name</span></span>       | <span data-ttu-id="8c92d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c92d-130">Type</span></span> | <span data-ttu-id="8c92d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c92d-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c92d-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c92d-132">Authorization</span></span>  | <span data-ttu-id="8c92d-133">string</span><span class="sxs-lookup"><span data-stu-id="8c92d-133">string</span></span>  | <span data-ttu-id="8c92d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c92d-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c92d-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c92d-136">Request body</span></span>
<span data-ttu-id="8c92d-137">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="8c92d-137">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="8c92d-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c92d-138">Property</span></span> | <span data-ttu-id="8c92d-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c92d-139">Type</span></span> | <span data-ttu-id="8c92d-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c92d-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c92d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8c92d-141">displayName</span></span> | <span data-ttu-id="8c92d-142">string</span><span class="sxs-lookup"><span data-stu-id="8c92d-142">string</span></span> | <span data-ttu-id="8c92d-143">O nome para exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="8c92d-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="8c92d-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c92d-144">Required.</span></span> |
| <span data-ttu-id="8c92d-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="8c92d-145">mailEnabled</span></span> | <span data-ttu-id="8c92d-146">booliano</span><span class="sxs-lookup"><span data-stu-id="8c92d-146">boolean</span></span> | <span data-ttu-id="8c92d-147">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="8c92d-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="8c92d-148">Defina isto como **true**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8c92d-148">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="8c92d-149">Defina como **false**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="8c92d-149">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="8c92d-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c92d-150">Required.</span></span> |
| <span data-ttu-id="8c92d-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8c92d-151">mailNickname</span></span> | <span data-ttu-id="8c92d-152">string</span><span class="sxs-lookup"><span data-stu-id="8c92d-152">string</span></span> | <span data-ttu-id="8c92d-153">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="8c92d-153">The mail alias for the group.</span></span> <span data-ttu-id="8c92d-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c92d-154">Required.</span></span> |
| <span data-ttu-id="8c92d-155">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="8c92d-155">securityEnabled</span></span> | <span data-ttu-id="8c92d-156">booliano</span><span class="sxs-lookup"><span data-stu-id="8c92d-156">boolean</span></span> | <span data-ttu-id="8c92d-157">Defina como **true** para grupos habilitados para segurança.</span><span class="sxs-lookup"><span data-stu-id="8c92d-157">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="8c92d-158">Definir isto como **true**, se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="8c92d-158">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="8c92d-159">Defina isto como **false**, se estiver criando um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8c92d-159">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="8c92d-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c92d-160">Required.</span></span> |
| <span data-ttu-id="8c92d-161">owners</span><span class="sxs-lookup"><span data-stu-id="8c92d-161">owners</span></span> | <span data-ttu-id="8c92d-162">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c92d-162">string collection</span></span> | <span data-ttu-id="8c92d-163">Esta propriedade representa os proprietários do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="8c92d-163">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="8c92d-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8c92d-164">Optional.</span></span> |
| <span data-ttu-id="8c92d-165">membros</span><span class="sxs-lookup"><span data-stu-id="8c92d-165">members</span></span> | <span data-ttu-id="8c92d-166">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c92d-166">string collection</span></span> | <span data-ttu-id="8c92d-167">Esta propriedade representa os membros do grupo na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="8c92d-167">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="8c92d-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8c92d-168">Optional.</span></span> |


<span data-ttu-id="8c92d-169">Especifique a propriedade **groupTypes**, se estiver criando um Grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="8c92d-169">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="8c92d-170">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="8c92d-170">groupTypes options</span></span>

| <span data-ttu-id="8c92d-171">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="8c92d-171">Type of group</span></span> | <span data-ttu-id="8c92d-172">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="8c92d-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="8c92d-173">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="8c92d-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="8c92d-174">"Unified"</span><span class="sxs-lookup"><span data-stu-id="8c92d-174">"Unified"</span></span> |
| <span data-ttu-id="8c92d-175">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="8c92d-175">Dynamic</span></span> | <span data-ttu-id="8c92d-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="8c92d-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="8c92d-177">Segurança</span><span class="sxs-lookup"><span data-stu-id="8c92d-177">Security</span></span> | <span data-ttu-id="8c92d-178">Não defina.</span><span class="sxs-lookup"><span data-stu-id="8c92d-178">Do not set.</span></span> |


><span data-ttu-id="8c92d-179">**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="8c92d-179">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="8c92d-180">Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.</span><span class="sxs-lookup"><span data-stu-id="8c92d-180">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="8c92d-p115">Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="8c92d-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="8c92d-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c92d-183">Response</span></span>
<span data-ttu-id="8c92d-184">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c92d-184">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c92d-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c92d-185">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="8c92d-186">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="8c92d-186">Request 1</span></span>
<span data-ttu-id="8c92d-187">A primeira solicitação de exemplo cria um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8c92d-187">The following is an example of a request that creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
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

#### <a name="response-1"></a><span data-ttu-id="8c92d-188">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="8c92d-188">Response 1</span></span>
<span data-ttu-id="8c92d-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c92d-189">The following is an example of the response.</span></span>
><span data-ttu-id="8c92d-190">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c92d-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c92d-191">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c92d-191">All default properties are returned from the actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
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

#### <a name="request-2"></a><span data-ttu-id="8c92d-192">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="8c92d-192">Request 2</span></span>
<span data-ttu-id="8c92d-193">A segunda solicitação de exemplo cria um Grupo do Office 365 com um proprietário especificado.</span><span class="sxs-lookup"><span data-stu-id="8c92d-193">The second example request creates an Office 365 group with an owner specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="8c92d-194">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="8c92d-194">Response 2</span></span>
<span data-ttu-id="8c92d-195">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="8c92d-195">The following is an example of a response to a  event.</span></span> <span data-ttu-id="8c92d-196">Ele inclui apenas propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="8c92d-196">It includes only default properties.</span></span> <span data-ttu-id="8c92d-197">Posteriormente, você pode obter a propriedade de navegação **owners** do grupo para verificar os detalhes do proprietário.</span><span class="sxs-lookup"><span data-stu-id="8c92d-197">You can subsequenty get the **owners** navigation property of the group to verify the details of the owner.</span></span> 
><span data-ttu-id="8c92d-198">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c92d-198">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c92d-199">Todas as propriedades padrão serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c92d-199">All default properties are returned from the actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner",
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
  "tocPath": ""
}-->

---
title: Criar grupo
description: 'Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 2a3e0e20622db47d410b578249df94f3354e75ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981543"
---
# <a name="create-group"></a><span data-ttu-id="4f04f-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="4f04f-104">Create group</span></span>
<span data-ttu-id="4f04f-p102">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="4f04f-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="4f04f-107">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="4f04f-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="4f04f-108">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="4f04f-108">Dynamic group</span></span>
* <span data-ttu-id="4f04f-109">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="4f04f-109">Security group</span></span>

> <span data-ttu-id="4f04f-p103">**Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4f04f-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f04f-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f04f-112">Permissions</span></span>
<span data-ttu-id="4f04f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f04f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f04f-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f04f-115">Permission type</span></span>      | <span data-ttu-id="4f04f-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f04f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f04f-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f04f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4f04f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f04f-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f04f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f04f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f04f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f04f-120">Not supported.</span></span>    |
|<span data-ttu-id="4f04f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f04f-121">Application</span></span> | <span data-ttu-id="4f04f-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f04f-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f04f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f04f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="4f04f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f04f-124">Request headers</span></span>
| <span data-ttu-id="4f04f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4f04f-125">Name</span></span>       | <span data-ttu-id="4f04f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f04f-126">Type</span></span> | <span data-ttu-id="4f04f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f04f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f04f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f04f-128">Authorization</span></span>  | <span data-ttu-id="4f04f-129">string</span><span class="sxs-lookup"><span data-stu-id="4f04f-129">string</span></span>  | <span data-ttu-id="4f04f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f04f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f04f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f04f-132">Request body</span></span>
<span data-ttu-id="4f04f-133">A tabela a seguir mostra as propriedades do [grupo de](../resources/group.md) recurso para especificar quando você cria um grupo.</span><span class="sxs-lookup"><span data-stu-id="4f04f-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="4f04f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f04f-134">Property</span></span> | <span data-ttu-id="4f04f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f04f-135">Type</span></span> | <span data-ttu-id="4f04f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f04f-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f04f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4f04f-137">displayName</span></span> | <span data-ttu-id="4f04f-138">string</span><span class="sxs-lookup"><span data-stu-id="4f04f-138">string</span></span> | <span data-ttu-id="4f04f-139">O nome de exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="4f04f-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="4f04f-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f04f-140">Required.</span></span> |
| <span data-ttu-id="4f04f-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4f04f-141">mailEnabled</span></span> | <span data-ttu-id="4f04f-142">booliano</span><span class="sxs-lookup"><span data-stu-id="4f04f-142">boolean</span></span> | <span data-ttu-id="4f04f-143">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="4f04f-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="4f04f-144">Defina como **true** se criando um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4f04f-144">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="4f04f-145">Defina como **false** se criando dinâmico ou grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="4f04f-145">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="4f04f-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f04f-146">Required.</span></span> |
| <span data-ttu-id="4f04f-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4f04f-147">mailNickname</span></span> | <span data-ttu-id="4f04f-148">string</span><span class="sxs-lookup"><span data-stu-id="4f04f-148">string</span></span> | <span data-ttu-id="4f04f-149">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="4f04f-149">The mail alias for the group.</span></span> <span data-ttu-id="4f04f-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f04f-150">Required.</span></span> |
| <span data-ttu-id="4f04f-151">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4f04f-151">securityEnabled</span></span> | <span data-ttu-id="4f04f-152">booliano</span><span class="sxs-lookup"><span data-stu-id="4f04f-152">boolean</span></span> | <span data-ttu-id="4f04f-153">Defina como **true** para grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="4f04f-153">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="4f04f-154">Defina isso como **true** se a criação de um grupo de segurança ou dinâmico.</span><span class="sxs-lookup"><span data-stu-id="4f04f-154">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="4f04f-155">Defina como **false** se criando um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4f04f-155">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="4f04f-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f04f-156">Required.</span></span> |
| <span data-ttu-id="4f04f-157">owners</span><span class="sxs-lookup"><span data-stu-id="4f04f-157">owners</span></span> | <span data-ttu-id="4f04f-158">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f04f-158">string collection</span></span> | <span data-ttu-id="4f04f-159">Essa propriedade representa os proprietários do grupo no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="4f04f-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="4f04f-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4f04f-160">Optional.</span></span> |
| <span data-ttu-id="4f04f-161">membros</span><span class="sxs-lookup"><span data-stu-id="4f04f-161">members</span></span> | <span data-ttu-id="4f04f-162">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f04f-162">string collection</span></span> | <span data-ttu-id="4f04f-163">Essa propriedade representa os membros do grupo no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="4f04f-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="4f04f-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4f04f-164">Optional.</span></span> |


<span data-ttu-id="4f04f-165">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="4f04f-165">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="4f04f-166">Opções de groupTypes</span><span class="sxs-lookup"><span data-stu-id="4f04f-166">groupTypes options</span></span>

| <span data-ttu-id="4f04f-167">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="4f04f-167">Type of group</span></span> | <span data-ttu-id="4f04f-168">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="4f04f-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="4f04f-169">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="4f04f-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="4f04f-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="4f04f-170">"Unified"</span></span> |
| <span data-ttu-id="4f04f-171">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="4f04f-171">Dynamic</span></span> | <span data-ttu-id="4f04f-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="4f04f-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="4f04f-173">Segurança</span><span class="sxs-lookup"><span data-stu-id="4f04f-173">Security</span></span> | <span data-ttu-id="4f04f-174">Não defina.</span><span class="sxs-lookup"><span data-stu-id="4f04f-174">Do not set.</span></span> |


><span data-ttu-id="4f04f-175">**Observação:** criar um grupo do Office 365 programaticamente sem um contexto do usuário e sem a especificação de proprietários criará o grupo anônimo.</span><span class="sxs-lookup"><span data-stu-id="4f04f-175">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="4f04f-176">Isso pode resultar no site do SharePoint Online associado não está sendo criado automaticamente até que ainda mais a ação manual é realizada.</span><span class="sxs-lookup"><span data-stu-id="4f04f-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="4f04f-p113">Especifique outras propriedades graváveis conforme necessário para o seu grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="4f04f-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="4f04f-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f04f-179">Response</span></span>
<span data-ttu-id="4f04f-180">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f04f-180">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f04f-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f04f-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="4f04f-182">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="4f04f-182">Request 1</span></span>
<span data-ttu-id="4f04f-183">A primeira solicitação de exemplo cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4f04f-183">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="4f04f-184">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="4f04f-184">Response 1</span></span>
<span data-ttu-id="4f04f-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f04f-185">The following is an example of the response.</span></span>
><span data-ttu-id="4f04f-186">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4f04f-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f04f-187">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f04f-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a><span data-ttu-id="4f04f-188">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="4f04f-188">Request 2</span></span>
<span data-ttu-id="4f04f-189">A segunda solicitação de exemplo cria um grupo do Office 365 com proprietários especificados.</span><span class="sxs-lookup"><span data-stu-id="4f04f-189">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="4f04f-190">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="4f04f-190">Response 2</span></span>
<span data-ttu-id="4f04f-191">O exemplo a seguir é um exemplo da resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="4f04f-191">The following is an example of the successful response.</span></span>
><span data-ttu-id="4f04f-192">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4f04f-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f04f-193">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f04f-193">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
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

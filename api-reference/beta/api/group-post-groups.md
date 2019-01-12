---
title: Criar grupo
description: 'Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: d1ce182a0122f621ccd1ea464df7a734bb89f24c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991157"
---
# <a name="create-group"></a><span data-ttu-id="7d237-104">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="7d237-104">Create group</span></span>

> <span data-ttu-id="7d237-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d237-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d237-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d237-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d237-107">Use essa API para criar um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d237-107">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="7d237-108">Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="7d237-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="7d237-109">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="7d237-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="7d237-110">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="7d237-110">Dynamic group</span></span>
* <span data-ttu-id="7d237-111">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="7d237-111">Security group</span></span>

> <span data-ttu-id="7d237-112">**Observação**: para criar uma [equipe](../resources/team.md), primeiro criar um grupo e adicionar uma equipe a ela, consulte [Criar equipe](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="7d237-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d237-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d237-113">Permissions</span></span>
<span data-ttu-id="7d237-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d237-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d237-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d237-116">Permission type</span></span>      | <span data-ttu-id="7d237-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d237-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d237-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d237-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7d237-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d237-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d237-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d237-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d237-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d237-121">Not supported.</span></span>    |
|<span data-ttu-id="7d237-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d237-122">Application</span></span> | <span data-ttu-id="7d237-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d237-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d237-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d237-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7d237-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d237-125">Request headers</span></span>
| <span data-ttu-id="7d237-126">Nome</span><span class="sxs-lookup"><span data-stu-id="7d237-126">Name</span></span>       | <span data-ttu-id="7d237-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d237-127">Type</span></span> | <span data-ttu-id="7d237-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d237-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d237-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d237-129">Authorization</span></span>  | <span data-ttu-id="7d237-130">string</span><span class="sxs-lookup"><span data-stu-id="7d237-130">string</span></span>  | <span data-ttu-id="7d237-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d237-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d237-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d237-133">Request body</span></span>
<span data-ttu-id="7d237-134">A tabela a seguir mostra as propriedades do [grupo de](../resources/group.md) recurso para especificar quando você cria um grupo.</span><span class="sxs-lookup"><span data-stu-id="7d237-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7d237-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d237-135">Property</span></span> | <span data-ttu-id="7d237-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d237-136">Type</span></span> | <span data-ttu-id="7d237-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d237-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d237-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7d237-138">displayName</span></span> | <span data-ttu-id="7d237-139">string</span><span class="sxs-lookup"><span data-stu-id="7d237-139">string</span></span> | <span data-ttu-id="7d237-140">O nome de exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="7d237-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="7d237-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d237-141">Required.</span></span> |
| <span data-ttu-id="7d237-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7d237-142">mailEnabled</span></span> | <span data-ttu-id="7d237-143">booliano</span><span class="sxs-lookup"><span data-stu-id="7d237-143">boolean</span></span> | <span data-ttu-id="7d237-144">Defina como **true** para grupos habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="7d237-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="7d237-145">Defina como **true** se criando um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d237-145">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="7d237-146">Defina como **false** se criando dinâmico ou grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="7d237-146">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="7d237-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d237-147">Required.</span></span> |
| <span data-ttu-id="7d237-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7d237-148">mailNickname</span></span> | <span data-ttu-id="7d237-149">string</span><span class="sxs-lookup"><span data-stu-id="7d237-149">string</span></span> | <span data-ttu-id="7d237-150">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="7d237-150">The mail alias for the group.</span></span> <span data-ttu-id="7d237-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d237-151">Required.</span></span> |
| <span data-ttu-id="7d237-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7d237-152">securityEnabled</span></span> | <span data-ttu-id="7d237-153">booliano</span><span class="sxs-lookup"><span data-stu-id="7d237-153">boolean</span></span> | <span data-ttu-id="7d237-154">Defina como **true** para grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="7d237-154">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="7d237-155">Defina isso como **true** se a criação de um grupo de segurança ou dinâmico.</span><span class="sxs-lookup"><span data-stu-id="7d237-155">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="7d237-156">Defina como **false** se criando um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d237-156">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="7d237-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d237-157">Required.</span></span> |
| <span data-ttu-id="7d237-158">owners</span><span class="sxs-lookup"><span data-stu-id="7d237-158">owners</span></span> | <span data-ttu-id="7d237-159">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d237-159">string collection</span></span> | <span data-ttu-id="7d237-160">Essa propriedade representa os proprietários do grupo no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="7d237-160">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="7d237-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7d237-161">Optional.</span></span> |
| <span data-ttu-id="7d237-162">membros</span><span class="sxs-lookup"><span data-stu-id="7d237-162">members</span></span> | <span data-ttu-id="7d237-163">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d237-163">string collection</span></span> | <span data-ttu-id="7d237-164">Essa propriedade representa os membros do grupo no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="7d237-164">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="7d237-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7d237-165">Optional.</span></span> |

<span data-ttu-id="7d237-166">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="7d237-166">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="7d237-167">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="7d237-167">Type of group</span></span> | <span data-ttu-id="7d237-168">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="7d237-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="7d237-169">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="7d237-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="7d237-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="7d237-170">"Unified"</span></span> |
| <span data-ttu-id="7d237-171">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="7d237-171">Dynamic</span></span> | <span data-ttu-id="7d237-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="7d237-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="7d237-173">Segurança</span><span class="sxs-lookup"><span data-stu-id="7d237-173">Security</span></span> | <span data-ttu-id="7d237-174">Não defina.</span><span class="sxs-lookup"><span data-stu-id="7d237-174">Do not set.</span></span> |

<span data-ttu-id="7d237-175">Desde que o recurso de **grupo** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `POST` operação e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="7d237-175">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7d237-176">**Observação:** Criar um grupo do Office 365 programaticamente sem um contexto do usuário e sem a especificação de proprietários anonimamente criará o grupo.</span><span class="sxs-lookup"><span data-stu-id="7d237-176">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="7d237-177">Isso pode resultar no site do SharePoint Online associado não está sendo criado automaticamente até que ainda mais a ação manual é realizada.</span><span class="sxs-lookup"><span data-stu-id="7d237-177">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7d237-p113">Especifique outras propriedades graváveis conforme necessário para o seu grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7d237-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7d237-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d237-180">Response</span></span>
<span data-ttu-id="7d237-181">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d237-181">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d237-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d237-182">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="7d237-183">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="7d237-183">Request 1</span></span>
<span data-ttu-id="7d237-184">A primeira solicitação de exemplo cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d237-184">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a><span data-ttu-id="7d237-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d237-185">Response</span></span>
<span data-ttu-id="7d237-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d237-186">The following is an example of the response.</span></span>
><span data-ttu-id="7d237-187">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d237-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7d237-188">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d237-188">All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="7d237-189">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="7d237-189">Request 2</span></span>
<span data-ttu-id="7d237-190">A segunda solicitação de exemplo cria um grupo do Office 365 com proprietários especificados.</span><span class="sxs-lookup"><span data-stu-id="7d237-190">The second example request creates an Office 365 Group with owners specified.</span></span>
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

 #### <a name="response-2"></a><span data-ttu-id="7d237-191">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="7d237-191">Response 2</span></span>
<span data-ttu-id="7d237-192">O exemplo a seguir é um exemplo da resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="7d237-192">The following is an example of the successful response.</span></span>
><span data-ttu-id="7d237-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d237-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7d237-195">Confira também</span><span class="sxs-lookup"><span data-stu-id="7d237-195">See also</span></span>

- [<span data-ttu-id="7d237-196">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7d237-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7d237-197">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="7d237-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7d237-198">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="7d237-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

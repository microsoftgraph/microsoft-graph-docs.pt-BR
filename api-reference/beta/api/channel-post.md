---
title: Criar canal
description: Crie um novo canal em uma equipe, conforme especificado no corpo da solicitação.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 549d4a3657655c9ee8be6be6bb82fee9dc9d769e
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753785"
---
# <a name="create-channel"></a><span data-ttu-id="2b8d5-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="2b8d5-103">Create channel</span></span>

<span data-ttu-id="2b8d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b8d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b8d5-105">Criar um novo [canal](../resources/channel.md) em uma equipe, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b8d5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b8d5-106">Permissions</span></span>

<span data-ttu-id="2b8d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b8d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b8d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b8d5-109">Permission type</span></span>      | <span data-ttu-id="2b8d5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b8d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b8d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b8d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b8d5-112">Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2b8d5-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="2b8d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b8d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b8d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-114">Not supported.</span></span>    |
|<span data-ttu-id="2b8d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b8d5-115">Application</span></span> | <span data-ttu-id="2b8d5-116">Channel. Create. Group \*, Channel. Create, entrabalho. Migration. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2b8d5-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="2b8d5-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="2b8d5-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="2b8d5-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2b8d5-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b8d5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b8d5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="2b8d5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-121">Request headers</span></span>

| <span data-ttu-id="2b8d5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b8d5-122">Header</span></span>       | <span data-ttu-id="2b8d5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2b8d5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b8d5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b8d5-124">Authorization</span></span>  | <span data-ttu-id="2b8d5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b8d5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b8d5-127">Content-Type</span></span>  | <span data-ttu-id="2b8d5-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b8d5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-130">Request body</span></span>

<span data-ttu-id="2b8d5-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Channel](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="2b8d5-131">In the request body, supply a JSON representation of a [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2b8d5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b8d5-132">Response</span></span>

<span data-ttu-id="2b8d5-133">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-133">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="2b8d5-134">Se a solicitação não for bem-sucedida, este método retorna um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-134">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="2b8d5-135">Os seguintes são motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="2b8d5-135">The following are common reasons for this response:</span></span>

* <span data-ttu-id="2b8d5-136">**createdDateTime** é definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-136">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="2b8d5-137">**createdDateTime** está especificado corretamente, mas o atributo de instância **channelCreationMode** está ausente ou definido como um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-137">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="2b8d5-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2b8d5-138">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="2b8d5-139">Exemplo 1: criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="2b8d5-139">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="2b8d5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-140">Request</span></span>

<span data-ttu-id="2b8d5-141">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-141">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b8d5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b8d5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="2b8d5-143">C#</span><span class="sxs-lookup"><span data-stu-id="2b8d5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b8d5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b8d5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b8d5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b8d5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b8d5-146">Java</span><span class="sxs-lookup"><span data-stu-id="2b8d5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="2b8d5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b8d5-147">Response</span></span>

<span data-ttu-id="2b8d5-148">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-148">The following example shows the response.</span></span>

> <span data-ttu-id="2b8d5-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_from_group",
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="2b8d5-150">Exemplo 2: criar um canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="2b8d5-150">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="2b8d5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-151">Request</span></span>

<span data-ttu-id="2b8d5-152">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-152">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b8d5-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b8d5-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_private_channel_with_member"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Graph.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="2b8d5-154">C#</span><span class="sxs-lookup"><span data-stu-id="2b8d5-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-private-channel-with-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b8d5-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b8d5-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-private-channel-with-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b8d5-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b8d5-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-private-channel-with-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b8d5-157">Java</span><span class="sxs-lookup"><span data-stu-id="2b8d5-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-private-channel-with-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="2b8d5-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b8d5-158">Response</span></span>

<span data-ttu-id="2b8d5-159">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-159">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_private_channel_with_member",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:33b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="2b8d5-160">Exemplo 3: criar um canal no modo de migração</span><span class="sxs-lookup"><span data-stu-id="2b8d5-160">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="2b8d5-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-161">Request</span></span>

<span data-ttu-id="2b8d5-162">O exemplo a seguir mostra como criar um canal que será usado para importar mensagens.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-162">The following example shows how to create a channel that will be used for importing messages.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b8d5-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b8d5-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```
# <a name="c"></a>[<span data-ttu-id="2b8d5-164">C#</span><span class="sxs-lookup"><span data-stu-id="2b8d5-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-for-migration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b8d5-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b8d5-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-for-migration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b8d5-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b8d5-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-for-migration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b8d5-167">Java</span><span class="sxs-lookup"><span data-stu-id="2b8d5-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-for-migration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b8d5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b8d5-168">Response</span></span>

<span data-ttu-id="2b8d5-169">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-169">The following example shows the response.</span></span> <span data-ttu-id="2b8d5-170">O cabeçalho Content-Location na resposta especifica o caminho para o canal que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-170">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="2b8d5-171">Após o provisionamento, este canal pode ser usado para [Importar mensagens](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="2b8d5-171">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_for_migration",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 202 Accepted
Location: /teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/{channelId}/operations/{operationId}
Content-Location: /teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/{channelId}
```

### <a name="example-4-create-standard-channel-with-moderation-settings"></a><span data-ttu-id="2b8d5-172">Exemplo 4: criar um canal padrão com configurações de moderação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-172">Example 4: Create standard channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="2b8d5-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b8d5-173">Request</span></span>

<span data-ttu-id="2b8d5-174">O exemplo a seguir mostra uma solicitação para criar um canal padrão com configurações de moderação.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-174">The following example shows a request to create a standard channel with moderation settings.</span></span> <span data-ttu-id="2b8d5-175">Essa operação só pode ser executada para um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-175">This operation can only be performed for a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b8d5-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b8d5-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_with_moderation_settings"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "everyoneExceptGuests",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```
# <a name="c"></a>[<span data-ttu-id="2b8d5-177">C#</span><span class="sxs-lookup"><span data-stu-id="2b8d5-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-with-moderation-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b8d5-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b8d5-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-with-moderation-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b8d5-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b8d5-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-with-moderation-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b8d5-180">Java</span><span class="sxs-lookup"><span data-stu-id="2b8d5-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-with-moderation-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="2b8d5-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b8d5-181">Response</span></span>

<span data-ttu-id="2b8d5-182">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b8d5-182">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:12b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:12b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

## <a name="see-also"></a><span data-ttu-id="2b8d5-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="2b8d5-183">See also</span></span>

* [<span data-ttu-id="2b8d5-184">Concluir a migração de um canal</span><span class="sxs-lookup"><span data-stu-id="2b8d5-184">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="2b8d5-185">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2b8d5-185">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="2b8d5-186">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="2b8d5-186">Create team</span></span>](team-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

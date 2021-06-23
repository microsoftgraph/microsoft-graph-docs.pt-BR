---
title: Criar canal
description: Crie um novo canal em uma equipe, conforme especificado no corpo da solicitação.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cca7ba2cfd6f69c6bbfda080c94c31013018657e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059923"
---
# <a name="create-channel"></a><span data-ttu-id="ef4c9-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="ef4c9-103">Create channel</span></span>

<span data-ttu-id="ef4c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef4c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef4c9-105">Crie um novo [canal](../resources/channel.md) em uma equipe, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef4c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef4c9-106">Permissions</span></span>

<span data-ttu-id="ef4c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef4c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef4c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef4c9-109">Permission type</span></span>      | <span data-ttu-id="ef4c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef4c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef4c9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef4c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ef4c9-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef4c9-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ef4c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef4c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef4c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-114">Not supported.</span></span>    |
|<span data-ttu-id="ef4c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef4c9-115">Application</span></span> | <span data-ttu-id="ef4c9-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef4c9-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ef4c9-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ef4c9-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="ef4c9-p102">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

> <span data-ttu-id="ef4c9-120">**Observação**: no futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados usando o Teamwork.Migrate.All e/ou APIs de [migração.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="ef4c9-120">**Note**: In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="ef4c9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4c9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="ef4c9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-122">Request headers</span></span>

| <span data-ttu-id="ef4c9-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef4c9-123">Header</span></span>       | <span data-ttu-id="ef4c9-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ef4c9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef4c9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef4c9-125">Authorization</span></span>  | <span data-ttu-id="ef4c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef4c9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef4c9-128">Content-Type</span></span>  | <span data-ttu-id="ef4c9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef4c9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-131">Request body</span></span>

<span data-ttu-id="ef4c9-132">No corpo da solicitação, fornece uma representação JSON de um [objeto channel.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="ef4c9-132">In the request body, supply a JSON representation of a [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef4c9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c9-133">Response</span></span>

<span data-ttu-id="ef4c9-134">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="ef4c9-135">Se a solicitação não for bem-sucedida, este método retorna um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-135">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="ef4c9-136">Os seguintes são motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="ef4c9-136">The following are common reasons for this response:</span></span>

* <span data-ttu-id="ef4c9-137">**createdDateTime** é definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-137">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="ef4c9-138">**createdDateTime** é especificado corretamente, mas o atributo de instância **channelCreationMode** está ausente ou definido como um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-138">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="ef4c9-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ef4c9-139">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="ef4c9-140">Exemplo 1: Criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="ef4c9-140">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="ef4c9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-141">Request</span></span>

<span data-ttu-id="ef4c9-142">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-142">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="ef4c9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4c9-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef4c9-144">C#</span><span class="sxs-lookup"><span data-stu-id="ef4c9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef4c9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef4c9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef4c9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef4c9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef4c9-147">Java</span><span class="sxs-lookup"><span data-stu-id="ef4c9-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="ef4c9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c9-148">Response</span></span>

<span data-ttu-id="ef4c9-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-149">The following example shows the response.</span></span>

> <span data-ttu-id="ef4c9-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-150">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
  "id": "19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="ef4c9-151">Exemplo 2: Criar canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="ef4c9-151">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="ef4c9-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-152">Request</span></span>

<span data-ttu-id="ef4c9-153">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-153">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="ef4c9-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4c9-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef4c9-155">C#</span><span class="sxs-lookup"><span data-stu-id="ef4c9-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-private-channel-with-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef4c9-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef4c9-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-private-channel-with-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef4c9-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef4c9-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-private-channel-with-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef4c9-158">Java</span><span class="sxs-lookup"><span data-stu-id="ef4c9-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-private-channel-with-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="ef4c9-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c9-159">Response</span></span>

<span data-ttu-id="ef4c9-160">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-160">The following example shows the response.</span></span>

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

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="ef4c9-161">Exemplo 3: Criar um canal no modo de migração</span><span class="sxs-lookup"><span data-stu-id="ef4c9-161">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="ef4c9-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-162">Request</span></span>

<span data-ttu-id="ef4c9-163">O exemplo a seguir mostra como criar um canal que será usado para importar mensagens.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-163">The following example shows how to create a channel that will be used for importing messages.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Import_150958_99z",
  "description": "Import_150958_99z",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```


#### <a name="response"></a><span data-ttu-id="ef4c9-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c9-164">Response</span></span>

<span data-ttu-id="ef4c9-165">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-165">The following example shows the response.</span></span> <span data-ttu-id="ef4c9-166">O header Content-Location na resposta especifica o caminho para o canal que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-166">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="ef4c9-167">Depois de provisionado, esse canal pode ser usado para [importar mensagens](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="ef4c9-167">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_for_migration",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Location: /teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:987c7a9fbe6447ccb3ea31bcded5c75c@thread.tacv2",
    "createdDateTime": null,
    "displayName": "Import_150958_99z",
    "description": "Import_150958_99z",
    "isFavoriteByDefault": null,
    "email": null,
    "webUrl": null,
    "membershipType": null,
    "moderationSettings": null
}
```

### <a name="example-4-create-standard-channel-with-moderation-settings"></a><span data-ttu-id="ef4c9-168">Exemplo 4: Criar canal padrão com configurações de moderação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-168">Example 4: Create standard channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="ef4c9-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4c9-169">Request</span></span>

<span data-ttu-id="ef4c9-170">O exemplo a seguir mostra uma solicitação para criar um canal padrão com configurações de moderação.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-170">The following example shows a request to create a standard channel with moderation settings.</span></span> <span data-ttu-id="ef4c9-171">Essa operação só pode ser executada para um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-171">This operation can only be performed for a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="ef4c9-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4c9-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef4c9-173">C#</span><span class="sxs-lookup"><span data-stu-id="ef4c9-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-with-moderation-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef4c9-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef4c9-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-with-moderation-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef4c9-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef4c9-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-with-moderation-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef4c9-176">Java</span><span class="sxs-lookup"><span data-stu-id="ef4c9-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-with-moderation-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="ef4c9-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4c9-177">Response</span></span>

<span data-ttu-id="ef4c9-178">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4c9-178">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ef4c9-179">Confira também</span><span class="sxs-lookup"><span data-stu-id="ef4c9-179">See also</span></span>

* [<span data-ttu-id="ef4c9-180">Concluir a migração para um canal</span><span class="sxs-lookup"><span data-stu-id="ef4c9-180">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="ef4c9-181">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ef4c9-181">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="ef4c9-182">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="ef4c9-182">Create team</span></span>](team-post.md)

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

---
title: Criar canal
description: Crie um novo canal em uma equipe, conforme especificado no corpo da solicitação.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3aeb01c320fce4b7ba1b8085a579f5d9d55efc87
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705902"
---
# <a name="create-channel"></a><span data-ttu-id="ab70d-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="ab70d-103">Create channel</span></span>

<span data-ttu-id="ab70d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab70d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab70d-105">Criar um novo [canal](../resources/channel.md) em uma equipe, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab70d-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab70d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab70d-106">Permissions</span></span>

<span data-ttu-id="ab70d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab70d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab70d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab70d-109">Permission type</span></span>      | <span data-ttu-id="ab70d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab70d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab70d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab70d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab70d-112">Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab70d-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ab70d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab70d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab70d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab70d-114">Not supported.</span></span>    |
|<span data-ttu-id="ab70d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab70d-115">Application</span></span> | <span data-ttu-id="ab70d-116">Channel. Create. Group \*, Channel. Create, entrabalho. Migration. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab70d-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ab70d-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ab70d-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="ab70d-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ab70d-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ab70d-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ab70d-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ab70d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab70d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="ab70d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab70d-121">Request headers</span></span>

| <span data-ttu-id="ab70d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab70d-122">Header</span></span>       | <span data-ttu-id="ab70d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ab70d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab70d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab70d-124">Authorization</span></span>  | <span data-ttu-id="ab70d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab70d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab70d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab70d-127">Content-Type</span></span>  | <span data-ttu-id="ab70d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab70d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab70d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab70d-130">Request body</span></span>

<span data-ttu-id="ab70d-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Channel](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="ab70d-131">In the request body, supply a JSON representation of a [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab70d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab70d-132">Response</span></span>

<span data-ttu-id="ab70d-133">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab70d-133">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="ab70d-134">Se a solicitação não for bem-sucedida, este método retorna um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="ab70d-134">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="ab70d-135">Os seguintes são motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="ab70d-135">The following are common reasons for this response:</span></span>

* <span data-ttu-id="ab70d-136">**createdDateTime** é definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="ab70d-136">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="ab70d-137">**createdDateTime** está especificado corretamente, mas o atributo de instância **channelCreationMode** está ausente ou definido como um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="ab70d-137">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="ab70d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab70d-138">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="ab70d-139">Exemplo 1: criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="ab70d-139">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="ab70d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab70d-140">Request</span></span>

<span data-ttu-id="ab70d-141">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="ab70d-141">The following example shows a request to create a standard channel.</span></span>

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

---

#### <a name="response"></a><span data-ttu-id="ab70d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab70d-142">Response</span></span>

<span data-ttu-id="ab70d-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab70d-143">The following example shows the response.</span></span>

> <span data-ttu-id="ab70d-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab70d-144">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="ab70d-145">Exemplo 2: criar um canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="ab70d-145">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="ab70d-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab70d-146">Request</span></span>

<span data-ttu-id="ab70d-147">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="ab70d-147">The following example shows a request to create a private channel and add a user as an team owner.</span></span>

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

---

#### <a name="response"></a><span data-ttu-id="ab70d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab70d-148">Response</span></span>

<span data-ttu-id="ab70d-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab70d-149">The following example shows the response.</span></span>

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

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="ab70d-150">Exemplo 3: criar um canal no modo de migração</span><span class="sxs-lookup"><span data-stu-id="ab70d-150">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="ab70d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab70d-151">Request</span></span>

<span data-ttu-id="ab70d-152">O exemplo a seguir mostra como criar um canal que será usado para importar mensagens.</span><span class="sxs-lookup"><span data-stu-id="ab70d-152">The following example shows how to create a channel that will be used for importing messages.</span></span>

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

#### <a name="response"></a><span data-ttu-id="ab70d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab70d-153">Response</span></span>

<span data-ttu-id="ab70d-154">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab70d-154">The following example shows the response.</span></span> <span data-ttu-id="ab70d-155">O cabeçalho Content-Location na resposta especifica o caminho para o canal que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="ab70d-155">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="ab70d-156">Após o provisionamento, este canal pode ser usado para [Importar mensagens](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="ab70d-156">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
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

### <a name="example-4-create-standard-channel-with-moderation-settings"></a><span data-ttu-id="ab70d-157">Exemplo 4: criar um canal padrão com configurações de moderação</span><span class="sxs-lookup"><span data-stu-id="ab70d-157">Example 4: Create standard channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="ab70d-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab70d-158">Request</span></span>

<span data-ttu-id="ab70d-159">O exemplo a seguir mostra uma solicitação para criar um canal padrão com configurações de moderação.</span><span class="sxs-lookup"><span data-stu-id="ab70d-159">The following example shows a request to create a standard channel with moderation settings.</span></span> <span data-ttu-id="ab70d-160">Essa operação só pode ser executada para um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="ab70d-160">This operation can only be performed for a standard channel.</span></span>

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

---

#### <a name="response"></a><span data-ttu-id="ab70d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab70d-161">Response</span></span>

<span data-ttu-id="ab70d-162">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab70d-162">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ab70d-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="ab70d-163">See also</span></span>

* [<span data-ttu-id="ab70d-164">Concluir a migração de um canal</span><span class="sxs-lookup"><span data-stu-id="ab70d-164">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="ab70d-165">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ab70d-165">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="ab70d-166">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="ab70d-166">Create team</span></span>](team-post.md)

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

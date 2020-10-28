---
title: Criar canal
description: Crie um novo canal em uma equipe da Microsoft, conforme especificado no corpo da solicitação.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 41d0e74ef3e08102a5fb670159d0f7e51085817d
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782815"
---
# <a name="create-channel"></a><span data-ttu-id="1d2fb-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="1d2fb-103">Create channel</span></span>

<span data-ttu-id="1d2fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d2fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d2fb-105">Criar um novo [canal](../resources/channel.md) em uma equipe, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d2fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d2fb-106">Permissions</span></span>

<span data-ttu-id="1d2fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d2fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d2fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d2fb-109">Permission type</span></span>      | <span data-ttu-id="1d2fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d2fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d2fb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d2fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d2fb-112">Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1d2fb-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d2fb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d2fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d2fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-114">Not supported.</span></span>    |
|<span data-ttu-id="1d2fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d2fb-115">Application</span></span> | <span data-ttu-id="1d2fb-116">Channel. Create. Group \*, Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All, entrabalho. Migrate. All</span><span class="sxs-lookup"><span data-stu-id="1d2fb-116">Channel.Create.Group\*, Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All, Teamwork.Migrate.All</span></span>|

> <span data-ttu-id="1d2fb-117">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1d2fb-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="1d2fb-118">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="1d2fb-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d2fb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d2fb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="1d2fb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2fb-121">Request headers</span></span>

| <span data-ttu-id="1d2fb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d2fb-122">Header</span></span>       | <span data-ttu-id="1d2fb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1d2fb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d2fb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d2fb-124">Authorization</span></span>  | <span data-ttu-id="1d2fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d2fb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d2fb-127">Content-Type</span></span>  | <span data-ttu-id="1d2fb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d2fb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2fb-130">Request body</span></span>

<span data-ttu-id="1d2fb-131">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="1d2fb-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1d2fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2fb-132">Response</span></span>

<span data-ttu-id="1d2fb-133">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-133">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="1d2fb-134">Se a solicitação não tiver êxito, este método retornará um `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-134">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="1d2fb-135">Estes são os motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="1d2fb-135">The following are common reasons for this response:</span></span>

* <span data-ttu-id="1d2fb-136">**createdDateTime** está definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-136">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="1d2fb-137">**createdDateTime** está especificado corretamente, mas o atributo de instância **channelCreationMode** está ausente ou definido como um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-137">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="1d2fb-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d2fb-138">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="1d2fb-139">Exemplo 1: criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="1d2fb-139">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="1d2fb-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2fb-140">Request</span></span>

<span data-ttu-id="1d2fb-141">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-141">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d2fb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d2fb-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```

# <a name="c"></a>[<span data-ttu-id="1d2fb-143">C#</span><span class="sxs-lookup"><span data-stu-id="1d2fb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d2fb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d2fb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d2fb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d2fb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1d2fb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2fb-146">Response</span></span>

<span data-ttu-id="1d2fb-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-147">The following example shows the response.</span></span>

> <span data-ttu-id="1d2fb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="1d2fb-150">Exemplo 2: criar um canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="1d2fb-150">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="1d2fb-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2fb-151">Request</span></span>

<span data-ttu-id="1d2fb-152">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-152">The following example shows a request to create a private channel and add a user as an team owner.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d2fb-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d2fb-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{group_id}/channels
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
           "user@odata.bind":"https://graph.microsoft.com/beta/users('{user_id}')",
           "roles":["owner"]
        }
     ]
}
```

# <a name="c"></a>[<span data-ttu-id="1d2fb-154">C#</span><span class="sxs-lookup"><span data-stu-id="1d2fb-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d2fb-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d2fb-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d2fb-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d2fb-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="1d2fb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2fb-157">Response</span></span>

<span data-ttu-id="1d2fb-158">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-158">The following example shows the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('{group_id}')/channels/$entity",
    "id": "{channel_id}",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/{channel_id}/My%20First%20Private%20Channel?groupId={group_id}&tenantId={tenant_id}",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="1d2fb-159">Exemplo 3: criar um canal no modo de migração</span><span class="sxs-lookup"><span data-stu-id="1d2fb-159">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="1d2fb-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2fb-160">Request</span></span>

<span data-ttu-id="1d2fb-161">O exemplo a seguir mostra como criar um canal para mensagens importadas.</span><span class="sxs-lookup"><span data-stu-id="1d2fb-161">The following example shows how to create a channel for imported messages.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="1d2fb-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2fb-162">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams/{teamId}/channels/{channelId}/operations/{operationId}
Content-Location: /teams/{teamId}/channels/{channelId}
```

## <a name="see-also"></a><span data-ttu-id="1d2fb-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="1d2fb-163">See also</span></span>

* [<span data-ttu-id="1d2fb-164">Concluir a migração de um canal</span><span class="sxs-lookup"><span data-stu-id="1d2fb-164">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="1d2fb-165">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d2fb-165">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="1d2fb-166">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="1d2fb-166">Create team</span></span>](team-post.md)

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

---
title: Criar canal
description: Crie um novo canal no Microsoft Team, como especificado no corpo da solicitação.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 81507c205b4935f6d355b35526e84d627bbb665c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288575"
---
# <a name="create-channel"></a><span data-ttu-id="f29d0-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="f29d0-103">Create Channel</span></span>

<span data-ttu-id="f29d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f29d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f29d0-105">Criar um novo [canal](../resources/channel.md) no Microsoft Team, como especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f29d0-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="f29d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f29d0-106">Permissions</span></span>

<span data-ttu-id="f29d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f29d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f29d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f29d0-109">Permission type</span></span>      | <span data-ttu-id="f29d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f29d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f29d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f29d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f29d0-112">Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f29d0-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f29d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f29d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f29d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f29d0-114">Not supported.</span></span>    |
|<span data-ttu-id="f29d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f29d0-115">Application</span></span> | <span data-ttu-id="f29d0-116">Channel. Create. Group ([RSC](https://aka.ms/teams-rsc)), Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f29d0-116">Channel.Create.Group ([RSC](https://aka.ms/teams-rsc)), Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="f29d0-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="f29d0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f29d0-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="f29d0-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f29d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f29d0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="f29d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f29d0-120">Request headers</span></span>

| <span data-ttu-id="f29d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f29d0-121">Header</span></span>       | <span data-ttu-id="f29d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f29d0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f29d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f29d0-123">Authorization</span></span>  | <span data-ttu-id="f29d0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f29d0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f29d0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f29d0-126">Content-Type</span></span>  | <span data-ttu-id="f29d0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f29d0-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f29d0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f29d0-128">Request body</span></span>

<span data-ttu-id="f29d0-129">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="f29d0-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f29d0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29d0-130">Response</span></span>

<span data-ttu-id="f29d0-131">Se bem-sucedido, esse método retornará `201 Created` código de resposta e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f29d0-131">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f29d0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f29d0-132">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="f29d0-133">Exemplo 1: criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="f29d0-133">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="f29d0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f29d0-134">Request</span></span>

<span data-ttu-id="f29d0-135">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="f29d0-135">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="f29d0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f29d0-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f29d0-137">C#</span><span class="sxs-lookup"><span data-stu-id="f29d0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f29d0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f29d0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f29d0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f29d0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f29d0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29d0-140">Response</span></span>

<span data-ttu-id="f29d0-141">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f29d0-141">The following example shows the response.</span></span>

> <span data-ttu-id="f29d0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f29d0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="f29d0-144">Exemplo 2: criar um canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="f29d0-144">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="f29d0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f29d0-145">Request</span></span>

<span data-ttu-id="f29d0-146">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="f29d0-146">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="f29d0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f29d0-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{group_id}/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Teams.Core.channel",
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
# <a name="c"></a>[<span data-ttu-id="f29d0-148">C#</span><span class="sxs-lookup"><span data-stu-id="f29d0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f29d0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f29d0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f29d0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f29d0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f29d0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29d0-151">Response</span></span>

<span data-ttu-id="f29d0-152">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f29d0-152">The following example shows the response.</span></span>

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

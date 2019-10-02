---
title: Criar canal
description: Crie um novo canal no Microsoft Team, como especificado no corpo da solicitação.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 470e0da36be8cf1d68a55d723fee8f39c737ebac
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355915"
---
# <a name="create-channel"></a><span data-ttu-id="b4376-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="b4376-103">Create Channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4376-104">Criar um novo [canal](../resources/channel.md) no Microsoft Team, como especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4376-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4376-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4376-105">Permissions</span></span>

<span data-ttu-id="b4376-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4376-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4376-108">Permission type</span></span>      | <span data-ttu-id="b4376-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4376-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4376-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4376-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4376-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4376-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4376-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4376-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4376-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4376-113">Not supported.</span></span>    |
|<span data-ttu-id="b4376-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4376-114">Application</span></span> | <span data-ttu-id="b4376-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4376-115">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="b4376-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="b4376-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b4376-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="b4376-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b4376-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4376-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="b4376-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4376-119">Request headers</span></span>

| <span data-ttu-id="b4376-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4376-120">Header</span></span>       | <span data-ttu-id="b4376-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b4376-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4376-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4376-122">Authorization</span></span>  | <span data-ttu-id="b4376-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4376-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b4376-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4376-125">Content-Type</span></span>  | <span data-ttu-id="b4376-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4376-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4376-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4376-127">Request body</span></span>

<span data-ttu-id="b4376-128">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b4376-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b4376-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4376-129">Response</span></span>

<span data-ttu-id="b4376-130">Se bem-sucedido, esse método retornará `201 Created` código de resposta e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4376-130">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4376-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b4376-131">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="b4376-132">Exemplo 1: criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="b4376-132">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="b4376-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4376-133">Request</span></span>

<span data-ttu-id="b4376-134">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="b4376-134">The following example shows a request to create a standard channel.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4376-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4376-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4376-136">C#</span><span class="sxs-lookup"><span data-stu-id="b4376-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4376-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4376-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4376-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4376-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b4376-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4376-139">Response</span></span>

<span data-ttu-id="b4376-140">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4376-140">The following example shows the response.</span></span>

> <span data-ttu-id="b4376-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4376-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="b4376-143">Exemplo 2: criar um canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="b4376-143">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="b4376-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4376-144">Request</span></span>

<span data-ttu-id="b4376-145">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="b4376-145">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4376-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4376-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4376-147">C#</span><span class="sxs-lookup"><span data-stu-id="b4376-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4376-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4376-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4376-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4376-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4376-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4376-150">Response</span></span>

<span data-ttu-id="b4376-151">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4376-151">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
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

---
title: Criar canal
description: Crie um novo canal no Microsoft Team, como especificado no corpo da solicitação.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9e98e389882dfe2f6dbe55194c6e589829a6e6f4
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491585"
---
# <a name="create-channel"></a><span data-ttu-id="95c62-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="95c62-103">Create Channel</span></span>

<span data-ttu-id="95c62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95c62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c62-105">Criar um novo [canal](../resources/channel.md) no Microsoft Team, como especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95c62-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="95c62-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="95c62-106">Permissions</span></span>

<span data-ttu-id="95c62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95c62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95c62-109">Permission type</span></span>      | <span data-ttu-id="95c62-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95c62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95c62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95c62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95c62-112">Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="95c62-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="95c62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95c62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95c62-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c62-114">Not supported.</span></span>    |
|<span data-ttu-id="95c62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95c62-115">Application</span></span> | <span data-ttu-id="95c62-116">Channel. Create. Group \*, Channel. Create, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="95c62-116">Channel.Create.Group\*, Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="95c62-117">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="95c62-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="95c62-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="95c62-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="95c62-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="95c62-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="95c62-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95c62-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="95c62-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95c62-121">Request headers</span></span>

| <span data-ttu-id="95c62-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95c62-122">Header</span></span>       | <span data-ttu-id="95c62-123">Valor</span><span class="sxs-lookup"><span data-stu-id="95c62-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95c62-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="95c62-124">Authorization</span></span>  | <span data-ttu-id="95c62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95c62-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95c62-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95c62-127">Content-Type</span></span>  | <span data-ttu-id="95c62-128">application/json</span><span class="sxs-lookup"><span data-stu-id="95c62-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95c62-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95c62-129">Request body</span></span>

<span data-ttu-id="95c62-130">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="95c62-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="95c62-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c62-131">Response</span></span>

<span data-ttu-id="95c62-132">Se bem-sucedido, esse método retornará `201 Created` código de resposta e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c62-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95c62-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95c62-133">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="95c62-134">Exemplo 1: criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="95c62-134">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="95c62-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c62-135">Request</span></span>

<span data-ttu-id="95c62-136">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="95c62-136">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="95c62-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="95c62-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="95c62-138">C#</span><span class="sxs-lookup"><span data-stu-id="95c62-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95c62-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95c62-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95c62-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95c62-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="95c62-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c62-141">Response</span></span>

<span data-ttu-id="95c62-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="95c62-142">The following example shows the response.</span></span>

> <span data-ttu-id="95c62-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95c62-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="95c62-145">Exemplo 2: criar um canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="95c62-145">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="95c62-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c62-146">Request</span></span>

<span data-ttu-id="95c62-147">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="95c62-147">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="95c62-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="95c62-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="95c62-149">C#</span><span class="sxs-lookup"><span data-stu-id="95c62-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95c62-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95c62-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95c62-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95c62-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95c62-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c62-152">Response</span></span>

<span data-ttu-id="95c62-153">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="95c62-153">The following example shows the response.</span></span>

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

---
title: Obter canal
description: Recuperar as propriedades e os relacionamentos de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 829e6fbc00ea57ea238d33ef0c0a47952c0b720c
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705930"
---
# <a name="get-channel"></a><span data-ttu-id="d915d-103">Obter canal</span><span class="sxs-lookup"><span data-stu-id="d915d-103">Get channel</span></span>

<span data-ttu-id="d915d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d915d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d915d-105">Recuperar as propriedades e os relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="d915d-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d915d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d915d-106">Permissions</span></span>

<span data-ttu-id="d915d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d915d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d915d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d915d-109">Permission type</span></span>      | <span data-ttu-id="d915d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d915d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d915d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d915d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d915d-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d915d-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d915d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d915d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d915d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d915d-114">Not supported.</span></span>    |
|<span data-ttu-id="d915d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d915d-115">Application</span></span> | <span data-ttu-id="d915d-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d915d-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d915d-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d915d-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d915d-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d915d-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d915d-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d915d-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d915d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d915d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d915d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d915d-121">Optional query parameters</span></span>

<span data-ttu-id="d915d-122">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d915d-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d915d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d915d-123">Request headers</span></span>

| <span data-ttu-id="d915d-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d915d-124">Header</span></span>       | <span data-ttu-id="d915d-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d915d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d915d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d915d-126">Authorization</span></span>  | <span data-ttu-id="d915d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d915d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d915d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d915d-129">Request body</span></span>

<span data-ttu-id="d915d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d915d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d915d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d915d-131">Response</span></span>

<span data-ttu-id="d915d-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d915d-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d915d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d915d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d915d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d915d-134">Request</span></span>

<span data-ttu-id="d915d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d915d-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d915d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d915d-136">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

# <a name="c"></a>[<span data-ttu-id="d915d-137">C#</span><span class="sxs-lookup"><span data-stu-id="d915d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d915d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d915d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d915d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d915d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d915d-140">Java</span><span class="sxs-lookup"><span data-stu-id="d915d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d915d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d915d-141">Response</span></span>

<span data-ttu-id="d915d-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d915d-142">Here is an example of the response.</span></span>

><span data-ttu-id="d915d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d915d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value",
    "membershipType": "membership-type-value"
}
```

<span data-ttu-id="d915d-145">Aqui está um exemplo da resposta para um canal padrão com moderação de canal desativada.</span><span class="sxs-lookup"><span data-stu-id="d915d-145">Here is an example of the response for a standard channel with channel moderation off.</span></span>

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('8bb12236-b929-42e0-94a0-1c417466ebf8')/channels/$entity",
    "id": "19:d468258bc90f4a358361b5d73b89d39b@thread.skype",
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3Ad468258bc90f4a358361b5d73b89d39b%40thread.skype/General?groupId=8bb12236-b929-42e0-94a0-1c417466ebf8&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "everyone",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```

<span data-ttu-id="d915d-146">Veja a seguir um exemplo da resposta de um canal padrão com moderação de canal no.</span><span class="sxs-lookup"><span data-stu-id="d915d-146">Here is an example of the response for a standard channel with channel moderation on.</span></span>

><span data-ttu-id="d915d-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d915d-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d915d-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d915d-148">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('8bb12236-b929-42e0-94a0-1c417466ebf8')/channels/$entity",
    "id": "19:d468258bc90f4a358361b5d73b89d39b@thread.skype",
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3Ad468258bc90f4a358361b5d73b89d39b%40thread.skype/General?groupId=8bb12236-b929-42e0-94a0-1c417466ebf8&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "moderators",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```

<span data-ttu-id="d915d-149">Veja um exemplo da resposta de um canal privado.</span><span class="sxs-lookup"><span data-stu-id="d915d-149">Here is an example of the response for a private channel.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('8bb12236-b929-42e0-94a0-1c417466ebf8')/channels/$entity",
    "id": "19:d468258bc90f4a358361b5d73b89d39b@thread.skype",
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3Ad468258bc90f4a358361b5d73b89d39b%40thread.skype/General?groupId=8bb12236-b929-42e0-94a0-1c417466ebf8&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
    "membershipType": "private",
    "moderationSettings": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



---
title: Obter canal
description: Recuperar as propriedades e os relacionamentos de um canal.
author: nkramer
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a1fb315e7ac6e12bfa3111cf6e89466e19139641
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201117"
---
# <a name="get-channel"></a><span data-ttu-id="8d918-103">Obter canal</span><span class="sxs-lookup"><span data-stu-id="8d918-103">Get channel</span></span>

<span data-ttu-id="8d918-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d918-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d918-105">Recuperar as propriedades e os relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8d918-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d918-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d918-106">Permissions</span></span>

<span data-ttu-id="8d918-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d918-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d918-109">Permission type</span></span>      | <span data-ttu-id="8d918-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d918-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d918-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d918-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d918-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d918-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8d918-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d918-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d918-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d918-114">Not supported.</span></span>    |
|<span data-ttu-id="8d918-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d918-115">Application</span></span> | <span data-ttu-id="8d918-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d918-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="8d918-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8d918-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="8d918-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8d918-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8d918-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8d918-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d918-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d918-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d918-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d918-121">Optional query parameters</span></span>

<span data-ttu-id="8d918-122">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d918-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d918-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d918-123">Request headers</span></span>

| <span data-ttu-id="8d918-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d918-124">Header</span></span>       | <span data-ttu-id="8d918-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8d918-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d918-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d918-126">Authorization</span></span>  | <span data-ttu-id="8d918-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d918-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d918-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d918-129">Request body</span></span>

<span data-ttu-id="8d918-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d918-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d918-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d918-131">Response</span></span>

<span data-ttu-id="8d918-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d918-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d918-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d918-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d918-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d918-134">Request</span></span>

<span data-ttu-id="8d918-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d918-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```

### <a name="response"></a><span data-ttu-id="8d918-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d918-136">Response</span></span>

<span data-ttu-id="8d918-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d918-137">Here is an example of the response.</span></span>

><span data-ttu-id="8d918-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d918-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
    "createdDateTime": "2020-05-27T19:22:25.692Z",
    "displayName": "General",
    "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
    "membershipType": "standard"
}

```

<span data-ttu-id="8d918-139">Aqui está um exemplo da resposta para um canal padrão com moderação de canal desligada.</span><span class="sxs-lookup"><span data-stu-id="8d918-139">Here is an example of the response for a standard channel with channel moderation off.</span></span>

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

<span data-ttu-id="8d918-140">Aqui está um exemplo da resposta para um canal padrão com moderação de canal.</span><span class="sxs-lookup"><span data-stu-id="8d918-140">Here is an example of the response for a standard channel with channel moderation on.</span></span>

><span data-ttu-id="8d918-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d918-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="8d918-142">Aqui está um exemplo da resposta para um canal privado.</span><span class="sxs-lookup"><span data-stu-id="8d918-142">Here is an example of the response for a private channel.</span></span>

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



---
title: Adicionar membro ao canal
description: Adicionar membro ao canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d5d16691b859955b11292c1f9997be3cc4b366e3
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387889"
---
# <a name="add-member-to-channel"></a><span data-ttu-id="ef281-103">Adicionar membro ao canal</span><span class="sxs-lookup"><span data-stu-id="ef281-103">Add member to channel</span></span>

<span data-ttu-id="ef281-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef281-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef281-105">Adicionar um [conversationMember](../resources/conversationmember.md) a um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ef281-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span> <span data-ttu-id="ef281-106">Essa operação só é permitida para canais com um valor de **membershiptype** de `private` .</span><span class="sxs-lookup"><span data-stu-id="ef281-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef281-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ef281-107">Permissions</span></span>

<span data-ttu-id="ef281-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef281-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef281-110">Permission Type</span></span>|<span data-ttu-id="ef281-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef281-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ef281-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef281-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ef281-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef281-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="ef281-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef281-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef281-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef281-115">Not supported.</span></span>|
|<span data-ttu-id="ef281-116">Application</span><span class="sxs-lookup"><span data-stu-id="ef281-116">Application</span></span>| <span data-ttu-id="ef281-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef281-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef281-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef281-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{team-id}/channels/{channel-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="ef281-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef281-119">Request headers</span></span>

| <span data-ttu-id="ef281-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef281-120">Header</span></span>       | <span data-ttu-id="ef281-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef281-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef281-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef281-122">Authorization</span></span>  | <span data-ttu-id="ef281-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef281-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef281-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="ef281-125">Content-type</span></span> | <span data-ttu-id="ef281-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef281-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef281-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef281-128">Request body</span></span>

<span data-ttu-id="ef281-129">Inclua as propriedades a seguir no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef281-129">Include the following properties in the request body.</span></span>

| <span data-ttu-id="ef281-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef281-130">Property</span></span>   | <span data-ttu-id="ef281-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef281-131">Type</span></span> |<span data-ttu-id="ef281-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef281-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef281-133">funções</span><span class="sxs-lookup"><span data-stu-id="ef281-133">roles</span></span>|<span data-ttu-id="ef281-134">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef281-134">string collection</span></span>|<span data-ttu-id="ef281-135">A função para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ef281-135">The role for the user.</span></span> <span data-ttu-id="ef281-136">Deve ser `owner` ou vazio.</span><span class="sxs-lookup"><span data-stu-id="ef281-136">Must be `owner` or empty.</span></span>|
|<span data-ttu-id="ef281-137">user</span><span class="sxs-lookup"><span data-stu-id="ef281-137">user</span></span>|[<span data-ttu-id="ef281-138">user</span><span class="sxs-lookup"><span data-stu-id="ef281-138">user</span></span>](../resources/user.md)|<span data-ttu-id="ef281-139">O usuário a ser adicionado ao canal.</span><span class="sxs-lookup"><span data-stu-id="ef281-139">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="ef281-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef281-140">Response</span></span>

<span data-ttu-id="ef281-141">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef281-141">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef281-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ef281-142">Examples</span></span>

### <a name="example-1-add-a-member-to-a-channel"></a><span data-ttu-id="ef281-143">Exemplo 1: adicionar um membro a um canal</span><span class="sxs-lookup"><span data-stu-id="ef281-143">Example 1: Add a member to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="ef281-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef281-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
```

#### <a name="response"></a><span data-ttu-id="ef281-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef281-145">Response</span></span>

><span data-ttu-id="ef281-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef281-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="example-2-add-a-member-with-the-owner-role-to-a-channel"></a><span data-ttu-id="ef281-147">Exemplo 2: adicionar um membro com a função proprietário a um canal</span><span class="sxs-lookup"><span data-stu-id="ef281-147">Example 2: Add a member with the owner role to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="ef281-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef281-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->

```http
POST https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
Content-type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
}
```

#### <a name="response"></a><span data-ttu-id="ef281-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef281-149">Response</span></span>

<span data-ttu-id="ef281-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef281-150">Here is an example of the response.</span></span>

><span data-ttu-id="ef281-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef281-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="ef281-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="ef281-152">See also</span></span>

- [<span data-ttu-id="ef281-153">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="ef281-153">Add member to team</span></span>](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add member to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

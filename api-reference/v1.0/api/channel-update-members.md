---
title: Atualizar membro no canal
description: Atualizar a função de membro em um canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20c6acd623d3ca4a352902fd57a0bd8b1074134c
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387791"
---
# <a name="update-member-in-channel"></a><span data-ttu-id="d0ac9-103">Atualizar membro no canal</span><span class="sxs-lookup"><span data-stu-id="d0ac9-103">Update member in channel</span></span>

<span data-ttu-id="d0ac9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0ac9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0ac9-105">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="d0ac9-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="d0ac9-106">Essa operação só é permitida para canais com um valor de **membershiptype** de `private` .</span><span class="sxs-lookup"><span data-stu-id="d0ac9-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0ac9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0ac9-107">Permissions</span></span>

<span data-ttu-id="d0ac9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0ac9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ac9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0ac9-110">Permission Type</span></span>|<span data-ttu-id="d0ac9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0ac9-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="d0ac9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0ac9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0ac9-113">ChannelMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-113">ChannelMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="d0ac9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0ac9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0ac9-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0ac9-115">Not supported</span></span>|
|<span data-ttu-id="d0ac9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0ac9-116">Application</span></span>|<span data-ttu-id="d0ac9-117">ChannelMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-117">ChannelMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0ac9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0ac9-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="d0ac9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ac9-119">Request headers</span></span>

| <span data-ttu-id="d0ac9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0ac9-120">Header</span></span>       | <span data-ttu-id="d0ac9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d0ac9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0ac9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0ac9-122">Authorization</span></span>  | <span data-ttu-id="d0ac9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d0ac9-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="d0ac9-125">Content-type</span></span> | <span data-ttu-id="d0ac9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0ac9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ac9-128">Request body</span></span>

<span data-ttu-id="d0ac9-129">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-129">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="d0ac9-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0ac9-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0ac9-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0ac9-132">Property</span></span>   | <span data-ttu-id="d0ac9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0ac9-133">Type</span></span> |<span data-ttu-id="d0ac9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0ac9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0ac9-135">funções</span><span class="sxs-lookup"><span data-stu-id="d0ac9-135">roles</span></span>|<span data-ttu-id="d0ac9-136">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0ac9-136">string collection</span></span>|<span data-ttu-id="d0ac9-137">A função para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-137">The role for the user.</span></span> <span data-ttu-id="d0ac9-138">Deve ser `owner` ou vazio.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-138">Must be `owner` or empty.</span></span> <span data-ttu-id="d0ac9-139">Os usuários convidados são automaticamente carimbados com `guest` a função e esse valor não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-139">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="d0ac9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0ac9-140">Response</span></span>

<span data-ttu-id="d0ac9-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [conversationMember](../resources/conversationmember.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-141">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0ac9-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0ac9-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0ac9-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ac9-143">Request</span></span>

<span data-ttu-id="d0ac9-144">A seguir está uma solicitação para aplicar a `owner` função a um membro existente de um canal.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-144">The following is a request to apply the `owner` role to an existing member of a channel.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="d0ac9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0ac9-145">Response</span></span>

><span data-ttu-id="d0ac9-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0ac9-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
## <a name="see-also"></a><span data-ttu-id="d0ac9-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="d0ac9-147">See also</span></span>

- [<span data-ttu-id="d0ac9-148">Atualizar a função do membro em uma equipe</span><span class="sxs-lookup"><span data-stu-id="d0ac9-148">Update member's role in a team</span></span>](team-update-members.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of channel member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

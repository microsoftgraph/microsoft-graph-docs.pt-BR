---
title: Atualizar conversationMember
description: Atualize a função do conversationMember em uma equipe ou canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 526bb7e232ad18a87571673655fa15fa37c4c995
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700868"
---
# <a name="update-conversationmember"></a><span data-ttu-id="ed7db-103">Atualizar conversationMember</span><span class="sxs-lookup"><span data-stu-id="ed7db-103">Update conversationMember</span></span>

<span data-ttu-id="ed7db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed7db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed7db-105">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em uma [equipe](../resources/team.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ed7db-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed7db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed7db-106">Permissions</span></span>

<span data-ttu-id="ed7db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed7db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed7db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed7db-109">Permission Type</span></span>|<span data-ttu-id="ed7db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed7db-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ed7db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed7db-111">Delegated (work or school account)</span></span>| <span data-ttu-id="ed7db-112">No Teams: TeamMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="ed7db-112">In teams: TeamMember.ReadWrite.All.</span></span> <span data-ttu-id="ed7db-113">Em canais: ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="ed7db-113">In channels: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All.</span></span> |
|<span data-ttu-id="ed7db-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed7db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed7db-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ed7db-115">Not supported</span></span>|
|<span data-ttu-id="ed7db-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed7db-116">Application</span></span>| <span data-ttu-id="ed7db-117">No Teams: TeamMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="ed7db-117">In teams: TeamMember.ReadWrite.All.</span></span> <span data-ttu-id="ed7db-118">Em canais: ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="ed7db-118">In channels:  ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed7db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed7db-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed7db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed7db-120">Request headers</span></span>

| <span data-ttu-id="ed7db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed7db-121">Header</span></span>       | <span data-ttu-id="ed7db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed7db-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed7db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed7db-123">Authorization</span></span>  | <span data-ttu-id="ed7db-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed7db-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed7db-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed7db-126">Request body</span></span>

<span data-ttu-id="ed7db-127">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="ed7db-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="ed7db-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ed7db-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ed7db-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ed7db-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ed7db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed7db-130">Property</span></span>   | <span data-ttu-id="ed7db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed7db-131">Type</span></span> |<span data-ttu-id="ed7db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed7db-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed7db-133">funções</span><span class="sxs-lookup"><span data-stu-id="ed7db-133">roles</span></span>|<span data-ttu-id="ed7db-134">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed7db-134">string collection</span></span>|<span data-ttu-id="ed7db-135">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="ed7db-135">The roles for that user.</span></span> <span data-ttu-id="ed7db-136">Deve ser "proprietário" ou vazio.</span><span class="sxs-lookup"><span data-stu-id="ed7db-136">Must be "owner" or empty.</span></span> <span data-ttu-id="ed7db-137">Os usuários convidados devem sempre ter a função "convidado" e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="ed7db-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="ed7db-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed7db-138">Response</span></span>

<span data-ttu-id="ed7db-139">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed7db-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed7db-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed7db-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed7db-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed7db-141">Request</span></span>

<span data-ttu-id="ed7db-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed7db-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="ed7db-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed7db-143">Response</span></span>

<span data-ttu-id="ed7db-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed7db-144">Here is an example of the response.</span></span>

><span data-ttu-id="ed7db-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed7db-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

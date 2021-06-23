---
title: Atualizar conversationMember
description: Atualizar a função de conversationMember em uma equipe ou canal.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 094027c7c62e6077c3eced8e713cfe16e84c3444
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060587"
---
# <a name="update-conversationmember"></a><span data-ttu-id="cf96d-103">Atualizar conversationMember</span><span class="sxs-lookup"><span data-stu-id="cf96d-103">Update conversationMember</span></span>

<span data-ttu-id="cf96d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf96d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf96d-105">Atualize a função de [um conversationMember](../resources/conversationmember.md) em uma [equipe](../resources/team.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="cf96d-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf96d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf96d-106">Permissions</span></span>

<span data-ttu-id="cf96d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf96d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf96d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf96d-109">Permission Type</span></span>|<span data-ttu-id="cf96d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf96d-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="cf96d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf96d-111">Delegated (work or school account)</span></span>| <span data-ttu-id="cf96d-112">Em equipes: TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf96d-112">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="cf96d-113">Em canais: ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf96d-113">In channels: ChannelMember.ReadWrite.All</span></span>  |
|<span data-ttu-id="cf96d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf96d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf96d-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cf96d-115">Not supported</span></span>|
|<span data-ttu-id="cf96d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf96d-116">Application</span></span>| <span data-ttu-id="cf96d-117">Em equipes: TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf96d-117">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="cf96d-118">Em canais: ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf96d-118">In channels:  ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf96d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf96d-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cf96d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf96d-120">Request headers</span></span>

| <span data-ttu-id="cf96d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf96d-121">Header</span></span>       | <span data-ttu-id="cf96d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf96d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf96d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf96d-123">Authorization</span></span>  | <span data-ttu-id="cf96d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf96d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf96d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf96d-126">Request body</span></span>

<span data-ttu-id="cf96d-127">No corpo da solicitação, fornece os valores para que os campos relevantes atualizem.</span><span class="sxs-lookup"><span data-stu-id="cf96d-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="cf96d-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="cf96d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cf96d-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cf96d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cf96d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf96d-130">Property</span></span>   | <span data-ttu-id="cf96d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf96d-131">Type</span></span> |<span data-ttu-id="cf96d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf96d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf96d-133">funções</span><span class="sxs-lookup"><span data-stu-id="cf96d-133">roles</span></span>|<span data-ttu-id="cf96d-134">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf96d-134">string collection</span></span>|<span data-ttu-id="cf96d-135">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="cf96d-135">The roles for that user.</span></span> <span data-ttu-id="cf96d-136">Deve ser "proprietário" ou vazio.</span><span class="sxs-lookup"><span data-stu-id="cf96d-136">Must be "owner" or empty.</span></span> <span data-ttu-id="cf96d-137">Os usuários convidados sempre devem ter a função "convidado" e não podem mudar.</span><span class="sxs-lookup"><span data-stu-id="cf96d-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="cf96d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf96d-138">Response</span></span>

<span data-ttu-id="cf96d-139">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf96d-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf96d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf96d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf96d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf96d-141">Request</span></span>

<span data-ttu-id="cf96d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf96d-142">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="cf96d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf96d-143">Response</span></span>

<span data-ttu-id="cf96d-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf96d-144">Here is an example of the response.</span></span>

><span data-ttu-id="cf96d-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf96d-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

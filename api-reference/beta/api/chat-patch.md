---
title: Atualizar chat
description: Atualizar as propriedades de um objeto chat.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1fdc063c0e66e881656f9428078ffa2105bc7bb5
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706205"
---
# <a name="update-chat"></a><span data-ttu-id="0d113-103">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="0d113-103">Update chat</span></span>
<span data-ttu-id="0d113-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d113-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d113-105">Atualizar as propriedades de um objeto [chat](../resources/chat.md) .</span><span class="sxs-lookup"><span data-stu-id="0d113-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d113-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d113-106">Permissions</span></span>
<span data-ttu-id="0d113-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d113-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d113-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d113-109">Permission type</span></span>|<span data-ttu-id="0d113-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d113-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d113-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d113-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d113-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d113-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="0d113-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d113-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d113-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d113-114">Not supported.</span></span> |
|<span data-ttu-id="0d113-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d113-115">Application</span></span> | <span data-ttu-id="0d113-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d113-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d113-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d113-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="0d113-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d113-118">Request headers</span></span>
|<span data-ttu-id="0d113-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0d113-119">Name</span></span>|<span data-ttu-id="0d113-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d113-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d113-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d113-121">Authorization</span></span>|<span data-ttu-id="0d113-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d113-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0d113-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d113-124">Content-Type</span></span>|<span data-ttu-id="0d113-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d113-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d113-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d113-127">Request body</span></span>
<span data-ttu-id="0d113-128">No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chat.md) .</span><span class="sxs-lookup"><span data-stu-id="0d113-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="0d113-129">A tabela a seguir mostra as propriedades que podem ser usadas com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0d113-129">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="0d113-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d113-130">Property</span></span>|<span data-ttu-id="0d113-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d113-131">Type</span></span>|<span data-ttu-id="0d113-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d113-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d113-133">topic</span><span class="sxs-lookup"><span data-stu-id="0d113-133">topic</span></span>|<span data-ttu-id="0d113-134">String</span><span class="sxs-lookup"><span data-stu-id="0d113-134">String</span></span>|<span data-ttu-id="0d113-135">O título do chat.</span><span class="sxs-lookup"><span data-stu-id="0d113-135">The title of the chat.</span></span> <span data-ttu-id="0d113-136">Isso só pode ser definido para um chat com um valor de **chattype** de `group` .</span><span class="sxs-lookup"><span data-stu-id="0d113-136">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="0d113-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d113-137">Response</span></span>

<span data-ttu-id="0d113-138">Se bem-sucedido, este método retorna um `200 OK response` código e o recurso de **chat** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d113-138">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d113-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d113-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d113-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d113-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update",
}
```


### <a name="response"></a><span data-ttu-id="0d113-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d113-141">Response</span></span>
><span data-ttu-id="0d113-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d113-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title update",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:12:19.943Z",
    "chatType": "group"
}
```


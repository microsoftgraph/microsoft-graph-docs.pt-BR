---
title: Atualizar chat
description: Atualize as propriedades de um objeto de chat.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 099c0a25ff054f20e97ee6b63dbc50cab02a6ffb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777325"
---
# <a name="update-chat"></a><span data-ttu-id="5b6ea-103">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="5b6ea-103">Update chat</span></span>
<span data-ttu-id="5b6ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b6ea-105">Atualize as propriedades de um [objeto de chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="5b6ea-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6ea-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5b6ea-106">Permissions</span></span>
<span data-ttu-id="5b6ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b6ea-109">Permission type</span></span>|<span data-ttu-id="5b6ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b6ea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b6ea-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b6ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b6ea-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b6ea-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="5b6ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b6ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-114">Not supported.</span></span> |
|<span data-ttu-id="5b6ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b6ea-115">Application</span></span> | <span data-ttu-id="5b6ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b6ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6ea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="5b6ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6ea-118">Request headers</span></span>
|<span data-ttu-id="5b6ea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5b6ea-119">Name</span></span>|<span data-ttu-id="5b6ea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b6ea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b6ea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b6ea-121">Authorization</span></span>|<span data-ttu-id="5b6ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5b6ea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b6ea-124">Content-Type</span></span>|<span data-ttu-id="5b6ea-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b6ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6ea-127">Request body</span></span>
<span data-ttu-id="5b6ea-128">No corpo da solicitação, fornece uma representação JSON do [objeto chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="5b6ea-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="5b6ea-129">A tabela a seguir mostra as propriedades que podem ser usadas com essa ação.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-129">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="5b6ea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b6ea-130">Property</span></span>|<span data-ttu-id="5b6ea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b6ea-131">Type</span></span>|<span data-ttu-id="5b6ea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b6ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b6ea-133">topic</span><span class="sxs-lookup"><span data-stu-id="5b6ea-133">topic</span></span>|<span data-ttu-id="5b6ea-134">String</span><span class="sxs-lookup"><span data-stu-id="5b6ea-134">String</span></span>|<span data-ttu-id="5b6ea-135">O título do chat.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-135">The title of the chat.</span></span> <span data-ttu-id="5b6ea-136">Isso só pode ser definido para um chat com um **valor chatType** de `group` .</span><span class="sxs-lookup"><span data-stu-id="5b6ea-136">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="5b6ea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6ea-137">Response</span></span>

<span data-ttu-id="5b6ea-138">Se tiver êxito, este método retornará um `200 OK response` código e o recurso de **chat** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-138">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b6ea-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b6ea-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b6ea-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6ea-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update"
}
```


### <a name="response"></a><span data-ttu-id="5b6ea-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6ea-141">Response</span></span>
><span data-ttu-id="5b6ea-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5b6ea-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title update",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:12:19.943Z",
    "chatType": "group"
}
```


---
title: Atualizar chat
description: Atualize as propriedades de um objeto de chat.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 26ba26e65a96bac04aa418d418b4588ff53f0ffd
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971052"
---
# <a name="update-chat"></a><span data-ttu-id="1b254-103">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="1b254-103">Update chat</span></span>
<span data-ttu-id="1b254-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b254-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b254-105">Atualize as propriedades de um [objeto de chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="1b254-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b254-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b254-106">Permissions</span></span>
<span data-ttu-id="1b254-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b254-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b254-109">Permission type</span></span>|<span data-ttu-id="1b254-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b254-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b254-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b254-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b254-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b254-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="1b254-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b254-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b254-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b254-114">Not supported.</span></span> |
|<span data-ttu-id="1b254-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b254-115">Application</span></span> | <span data-ttu-id="1b254-116">ChatSettings.ReadWrite.Chat\*, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b254-116">ChatSettings.ReadWrite.Chat\*, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="1b254-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1b254-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="1b254-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b254-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="1b254-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b254-119">Request headers</span></span>
|<span data-ttu-id="1b254-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1b254-120">Name</span></span>|<span data-ttu-id="1b254-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b254-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b254-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b254-122">Authorization</span></span>|<span data-ttu-id="1b254-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b254-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1b254-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b254-125">Content-Type</span></span>|<span data-ttu-id="1b254-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b254-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b254-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b254-128">Request body</span></span>
<span data-ttu-id="1b254-129">No corpo da solicitação, fornece uma representação JSON do [objeto chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="1b254-129">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="1b254-130">A tabela a seguir mostra as propriedades que podem ser usadas com essa ação.</span><span class="sxs-lookup"><span data-stu-id="1b254-130">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="1b254-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b254-131">Property</span></span>|<span data-ttu-id="1b254-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b254-132">Type</span></span>|<span data-ttu-id="1b254-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b254-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b254-134">topic</span><span class="sxs-lookup"><span data-stu-id="1b254-134">topic</span></span>|<span data-ttu-id="1b254-135">String</span><span class="sxs-lookup"><span data-stu-id="1b254-135">String</span></span>|<span data-ttu-id="1b254-136">O título do chat.</span><span class="sxs-lookup"><span data-stu-id="1b254-136">The title of the chat.</span></span> <span data-ttu-id="1b254-137">Isso só pode ser definido para um chat com um **valor chatType** de `group` .</span><span class="sxs-lookup"><span data-stu-id="1b254-137">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="1b254-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b254-138">Response</span></span>

<span data-ttu-id="1b254-139">Se tiver êxito, este método retornará um `200 OK response` código e o recurso de **chat** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b254-139">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b254-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b254-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b254-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b254-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1b254-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b254-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update"
}
```
# <a name="c"></a>[<span data-ttu-id="1b254-143">C#</span><span class="sxs-lookup"><span data-stu-id="1b254-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b254-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b254-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b254-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b254-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b254-146">Java</span><span class="sxs-lookup"><span data-stu-id="1b254-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1b254-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b254-147">Response</span></span>
><span data-ttu-id="1b254-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b254-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "chatType": "group",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A1c5b01696d2e4a179c292bc9cf04e63b@thread.v2/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```


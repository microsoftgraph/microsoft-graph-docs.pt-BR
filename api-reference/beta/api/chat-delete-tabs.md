---
title: Excluir guia do chat
description: 'Remova (desempinar) uma guia do chat especificado. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 84509aff2efaf1c528c52b9e73744d6fada0ebb6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047298"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="11f5f-103">Excluir guia do chat</span><span class="sxs-lookup"><span data-stu-id="11f5f-103">Delete tab from chat</span></span>

<span data-ttu-id="11f5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11f5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11f5f-105">Remover (desempinar) uma guia do [chat especificado](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="11f5f-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

> <span data-ttu-id="11f5f-106">**Observação**: se o chat estiver associado a uma instância [onlineMeeting,](../resources/onlinemeeting.md) então, efetivamente, a guia será removida da reunião.</span><span class="sxs-lookup"><span data-stu-id="11f5f-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="11f5f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="11f5f-107">Permissions</span></span>
<span data-ttu-id="11f5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11f5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f5f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11f5f-110">Permission type</span></span>      | <span data-ttu-id="11f5f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11f5f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f5f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11f5f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="11f5f-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f5f-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="11f5f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11f5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f5f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11f5f-115">Not supported.</span></span>    |
|<span data-ttu-id="11f5f-116">Application</span><span class="sxs-lookup"><span data-stu-id="11f5f-116">Application</span></span> | <span data-ttu-id="11f5f-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f5f-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="11f5f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11f5f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="11f5f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11f5f-119">Request headers</span></span>
| <span data-ttu-id="11f5f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11f5f-120">Header</span></span>       | <span data-ttu-id="11f5f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="11f5f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11f5f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11f5f-122">Authorization</span></span>  | <span data-ttu-id="11f5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11f5f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11f5f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11f5f-125">Request body</span></span>
<span data-ttu-id="11f5f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11f5f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11f5f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="11f5f-127">Response</span></span>

<span data-ttu-id="11f5f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11f5f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11f5f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11f5f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="11f5f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11f5f-131">Request</span></span>
<span data-ttu-id="11f5f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11f5f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11f5f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="11f5f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```
# <a name="c"></a>[<span data-ttu-id="11f5f-134">C#</span><span class="sxs-lookup"><span data-stu-id="11f5f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tab-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11f5f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11f5f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tab-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11f5f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11f5f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tab-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11f5f-137">Java</span><span class="sxs-lookup"><span data-stu-id="11f5f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tab-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="11f5f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="11f5f-138">Response</span></span>
<span data-ttu-id="11f5f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11f5f-139">The following is an example of the response.</span></span> <span data-ttu-id="11f5f-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11f5f-140">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="11f5f-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="11f5f-141">See also</span></span>

- [<span data-ttu-id="11f5f-142">Excluir guia do canal</span><span class="sxs-lookup"><span data-stu-id="11f5f-142">Delete tab from channel</span></span>](channel-delete-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



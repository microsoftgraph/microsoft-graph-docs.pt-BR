---
title: Excluir guia do chat
description: 'Remova (desempinar) uma guia do chat especificado. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5168994cbafcb0f8bc51af0a4bfa6c17cb7cea6b
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971346"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="f5c04-103">Excluir guia do chat</span><span class="sxs-lookup"><span data-stu-id="f5c04-103">Delete tab from chat</span></span>

<span data-ttu-id="f5c04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5c04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c04-105">Remover (desempinar) uma guia do [chat especificado](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="f5c04-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

> <span data-ttu-id="f5c04-106">**Observação**: se o chat estiver associado a uma instância [onlineMeeting,](../resources/onlinemeeting.md) então, efetivamente, a guia será removida da reunião.</span><span class="sxs-lookup"><span data-stu-id="f5c04-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5c04-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5c04-107">Permissions</span></span>
<span data-ttu-id="f5c04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5c04-110">Permission type</span></span>      | <span data-ttu-id="f5c04-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5c04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5c04-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5c04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5c04-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5c04-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="f5c04-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5c04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5c04-115">Not supported.</span></span>    |
|<span data-ttu-id="f5c04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5c04-116">Application</span></span> | <span data-ttu-id="f5c04-117">TeamsTab.Delete.Chat *, TeamsTab.ReadWrite.Chat*, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5c04-117">TeamsTab.Delete.Chat *, TeamsTab.ReadWrite.Chat*, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |

> <span data-ttu-id="f5c04-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f5c04-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="f5c04-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="f5c04-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c04-120">Request headers</span></span>
| <span data-ttu-id="f5c04-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5c04-121">Header</span></span>       | <span data-ttu-id="f5c04-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5c04-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5c04-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5c04-123">Authorization</span></span>  | <span data-ttu-id="f5c04-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5c04-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5c04-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c04-126">Request body</span></span>
<span data-ttu-id="f5c04-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5c04-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5c04-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c04-128">Response</span></span>

<span data-ttu-id="f5c04-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c04-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5c04-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5c04-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5c04-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c04-132">Request</span></span>
<span data-ttu-id="f5c04-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c04-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5c04-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c04-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```
# <a name="c"></a>[<span data-ttu-id="f5c04-135">C#</span><span class="sxs-lookup"><span data-stu-id="f5c04-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tab-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5c04-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5c04-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tab-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5c04-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5c04-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tab-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5c04-138">Java</span><span class="sxs-lookup"><span data-stu-id="f5c04-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tab-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f5c04-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c04-139">Response</span></span>
<span data-ttu-id="f5c04-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c04-140">The following is an example of the response.</span></span> <span data-ttu-id="f5c04-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f5c04-141">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="f5c04-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="f5c04-142">See also</span></span>

- [<span data-ttu-id="f5c04-143">Excluir guia do canal</span><span class="sxs-lookup"><span data-stu-id="f5c04-143">Delete tab from channel</span></span>](channel-delete-tabs.md)

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



---
title: Excluir guia do chat
description: 'Remova (desempinar) uma guia do chat especificado. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70fb781618c094406948b52e4c8068163ad1808e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777584"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="85c99-103">Excluir guia do chat</span><span class="sxs-lookup"><span data-stu-id="85c99-103">Delete tab from chat</span></span>

<span data-ttu-id="85c99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85c99-105">Remover (desempinar) uma guia do [chat especificado](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="85c99-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

> <span data-ttu-id="85c99-106">**Observação**: se o chat estiver associado a uma instância [onlineMeeting,](../resources/onlinemeeting.md) então, efetivamente, a guia será removida da reunião.</span><span class="sxs-lookup"><span data-stu-id="85c99-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="85c99-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="85c99-107">Permissions</span></span>
<span data-ttu-id="85c99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85c99-110">Permission type</span></span>      | <span data-ttu-id="85c99-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85c99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85c99-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85c99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85c99-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c99-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="85c99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85c99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85c99-115">Not supported.</span></span>    |
|<span data-ttu-id="85c99-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85c99-116">Application</span></span> | <span data-ttu-id="85c99-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c99-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="85c99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85c99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="85c99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85c99-119">Request headers</span></span>
| <span data-ttu-id="85c99-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85c99-120">Header</span></span>       | <span data-ttu-id="85c99-121">Valor</span><span class="sxs-lookup"><span data-stu-id="85c99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85c99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85c99-122">Authorization</span></span>  | <span data-ttu-id="85c99-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85c99-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85c99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85c99-125">Request body</span></span>
<span data-ttu-id="85c99-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85c99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85c99-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="85c99-127">Response</span></span>

<span data-ttu-id="85c99-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85c99-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c99-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85c99-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="85c99-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85c99-131">Request</span></span>
<span data-ttu-id="85c99-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85c99-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```


### <a name="response"></a><span data-ttu-id="85c99-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="85c99-133">Response</span></span>
<span data-ttu-id="85c99-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85c99-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="85c99-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="85c99-135">See also</span></span>

- [<span data-ttu-id="85c99-136">Excluir guia do canal</span><span class="sxs-lookup"><span data-stu-id="85c99-136">Delete tab from channel</span></span>](channel-delete-tabs.md)

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



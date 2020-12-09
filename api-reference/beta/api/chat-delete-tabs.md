---
title: Excluir Guia de chat
description: 'Remover (Desafixar) uma guia do chat especificado. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c83e8c9d1c501b27c46a6df3958008fb4447c06b
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607468"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="21dee-103">Excluir Guia de chat</span><span class="sxs-lookup"><span data-stu-id="21dee-103">Delete tab from chat</span></span>

<span data-ttu-id="21dee-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="21dee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21dee-105">Remover (Desafixar) uma guia do [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="21dee-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="21dee-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="21dee-106">Permissions</span></span>
<span data-ttu-id="21dee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21dee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21dee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21dee-109">Permission type</span></span>      | <span data-ttu-id="21dee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21dee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21dee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21dee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="21dee-112">TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="21dee-112">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="21dee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21dee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21dee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21dee-114">Not supported.</span></span>    |
|<span data-ttu-id="21dee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21dee-115">Application</span></span> | <span data-ttu-id="21dee-116">TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="21dee-116">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="21dee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21dee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="21dee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21dee-118">Request headers</span></span>
| <span data-ttu-id="21dee-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21dee-119">Header</span></span>       | <span data-ttu-id="21dee-120">Valor</span><span class="sxs-lookup"><span data-stu-id="21dee-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21dee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="21dee-121">Authorization</span></span>  | <span data-ttu-id="21dee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21dee-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21dee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21dee-124">Request body</span></span>
<span data-ttu-id="21dee-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21dee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21dee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="21dee-126">Response</span></span>

<span data-ttu-id="21dee-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21dee-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21dee-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21dee-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="21dee-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21dee-130">Request</span></span>
<span data-ttu-id="21dee-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21dee-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```
### <a name="response"></a><span data-ttu-id="21dee-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="21dee-132">Response</span></span>
<span data-ttu-id="21dee-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21dee-133">The following is an example of the response.</span></span> <span data-ttu-id="21dee-134">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="21dee-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="21dee-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21dee-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="21dee-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="21dee-136">See also</span></span>

- [<span data-ttu-id="21dee-137">Excluir Guia do canal</span><span class="sxs-lookup"><span data-stu-id="21dee-137">Delete tab from channel</span></span>](channel-delete-tabs.md)

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



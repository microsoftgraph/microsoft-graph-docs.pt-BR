---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9ad696741d9dfa02fc6dabea43673b268dfe97f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052492"
---
# <a name="delete-call"></a><span data-ttu-id="1bc7b-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="1bc7b-103">Delete call</span></span>

<span data-ttu-id="1bc7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bc7b-105">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-105">Delete or hang up an active call.</span></span> <span data-ttu-id="1bc7b-106">Para chamadas de grupo, isso excluirá apenas sua etapa de chamada e a chamada de grupo subjacente continuará.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-106">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bc7b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bc7b-107">Permissions</span></span>

| <span data-ttu-id="1bc7b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bc7b-108">Permission type</span></span> | <span data-ttu-id="1bc7b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bc7b-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1bc7b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bc7b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bc7b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-111">Not Supported.</span></span>                         |
| <span data-ttu-id="1bc7b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bc7b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc7b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-113">Not Supported.</span></span>                         |
| <span data-ttu-id="1bc7b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bc7b-114">Application</span></span>                            | <span data-ttu-id="1bc7b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1bc7b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bc7b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1bc7b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc7b-117">Request headers</span></span>
| <span data-ttu-id="1bc7b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1bc7b-118">Name</span></span>          | <span data-ttu-id="1bc7b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bc7b-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1bc7b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bc7b-120">Authorization</span></span> | <span data-ttu-id="1bc7b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bc7b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc7b-123">Request body</span></span>
<span data-ttu-id="1bc7b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bc7b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bc7b-125">Response</span></span>
<span data-ttu-id="1bc7b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bc7b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bc7b-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1bc7b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc7b-129">Request</span></span>
<span data-ttu-id="1bc7b-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-130">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1bc7b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bc7b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[<span data-ttu-id="1bc7b-132">C#</span><span class="sxs-lookup"><span data-stu-id="1bc7b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bc7b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bc7b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bc7b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bc7b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bc7b-135">Java</span><span class="sxs-lookup"><span data-stu-id="1bc7b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1bc7b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bc7b-136">Response</span></span>

> <span data-ttu-id="1bc7b-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1bc7b-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="1bc7b-138">Notificação - término</span><span class="sxs-lookup"><span data-stu-id="1bc7b-138">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

##### <a name="notification---terminated"></a><span data-ttu-id="1bc7b-139">Notificação - encerrada</span><span class="sxs-lookup"><span data-stu-id="1bc7b-139">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "0"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b87ced1c3755462691122b1ccce65e7bb8688d35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987439"
---
# <a name="delete-call"></a><span data-ttu-id="9b00e-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="9b00e-103">Delete call</span></span>

<span data-ttu-id="9b00e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b00e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b00e-105">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="9b00e-105">Delete or hang up an active call.</span></span> <span data-ttu-id="9b00e-106">Para chamadas de grupo, isso só excluirá o trecho de chamada, e a chamada de grupo subjacente ainda continuará.</span><span class="sxs-lookup"><span data-stu-id="9b00e-106">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b00e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b00e-107">Permissions</span></span>

| <span data-ttu-id="9b00e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b00e-108">Permission type</span></span> | <span data-ttu-id="9b00e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b00e-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="9b00e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b00e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b00e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b00e-111">Not Supported.</span></span>                         |
| <span data-ttu-id="9b00e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b00e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b00e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b00e-113">Not Supported.</span></span>                         |
| <span data-ttu-id="9b00e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b00e-114">Application</span></span>                            | <span data-ttu-id="9b00e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9b00e-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="9b00e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b00e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /communications/calls/{id}
```
> <span data-ttu-id="9b00e-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="9b00e-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="9b00e-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="9b00e-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b00e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b00e-119">Request headers</span></span>
| <span data-ttu-id="9b00e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9b00e-120">Name</span></span>          | <span data-ttu-id="9b00e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b00e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9b00e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b00e-122">Authorization</span></span> | <span data-ttu-id="9b00e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b00e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b00e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b00e-125">Request body</span></span>
<span data-ttu-id="9b00e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b00e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b00e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b00e-127">Response</span></span>
<span data-ttu-id="9b00e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b00e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b00e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b00e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9b00e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b00e-131">Request</span></span>
<span data-ttu-id="9b00e-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b00e-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9b00e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b00e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[<span data-ttu-id="9b00e-134">C#</span><span class="sxs-lookup"><span data-stu-id="9b00e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b00e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b00e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b00e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b00e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b00e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b00e-137">Response</span></span>

> <span data-ttu-id="9b00e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b00e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="9b00e-140">Notificação-encerramento</span><span class="sxs-lookup"><span data-stu-id="9b00e-140">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="9b00e-141">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="9b00e-141">Notification - terminated</span></span>

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



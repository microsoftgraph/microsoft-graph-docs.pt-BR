---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3daec6791d183ee2443d6af694b6dd6c39470155
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006344"
---
# <a name="delete-call"></a><span data-ttu-id="76d05-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="76d05-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d05-104">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="76d05-104">Delete or hang up an active call.</span></span> <span data-ttu-id="76d05-105">Para chamadas de grupo, isso só excluirá o trecho de chamada, e a chamada de grupo subjacente ainda continuará.</span><span class="sxs-lookup"><span data-stu-id="76d05-105">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="76d05-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="76d05-106">Permissions</span></span>

| <span data-ttu-id="76d05-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76d05-107">Permission type</span></span> | <span data-ttu-id="76d05-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76d05-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="76d05-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76d05-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="76d05-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76d05-110">Not Supported.</span></span>                         |
| <span data-ttu-id="76d05-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76d05-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76d05-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76d05-112">Not Supported.</span></span>                         |
| <span data-ttu-id="76d05-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76d05-113">Application</span></span>                            | <span data-ttu-id="76d05-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76d05-114">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="76d05-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76d05-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /communications/calls/{id}
```
> <span data-ttu-id="76d05-116">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="76d05-116">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="76d05-117">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="76d05-117">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76d05-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76d05-118">Request headers</span></span>
| <span data-ttu-id="76d05-119">Nome</span><span class="sxs-lookup"><span data-stu-id="76d05-119">Name</span></span>          | <span data-ttu-id="76d05-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="76d05-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="76d05-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="76d05-121">Authorization</span></span> | <span data-ttu-id="76d05-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76d05-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76d05-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76d05-124">Request body</span></span>
<span data-ttu-id="76d05-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76d05-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76d05-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="76d05-126">Response</span></span>
<span data-ttu-id="76d05-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76d05-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76d05-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76d05-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="76d05-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76d05-130">Request</span></span>
<span data-ttu-id="76d05-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="76d05-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="76d05-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="76d05-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76d05-133">C#</span><span class="sxs-lookup"><span data-stu-id="76d05-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76d05-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76d05-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76d05-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76d05-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="76d05-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="76d05-136">Response</span></span>

> <span data-ttu-id="76d05-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76d05-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="76d05-139">Notificação-encerramento</span><span class="sxs-lookup"><span data-stu-id="76d05-139">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="76d05-140">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="76d05-140">Notification - terminated</span></span>

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

---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dbdaf4a0332c52e932031da29e0427c3b054763b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948540"
---
# <a name="delete-call"></a><span data-ttu-id="c98b2-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="c98b2-103">Delete call</span></span>

<span data-ttu-id="c98b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c98b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c98b2-105">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="c98b2-105">Delete or hang up an active call.</span></span> <span data-ttu-id="c98b2-106">Para chamadas de grupo, isso excluirá apenas sua etapa de chamada e a chamada de grupo subjacente continuará.</span><span class="sxs-lookup"><span data-stu-id="c98b2-106">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="c98b2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c98b2-107">Permissions</span></span>

| <span data-ttu-id="c98b2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c98b2-108">Permission type</span></span> | <span data-ttu-id="c98b2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c98b2-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="c98b2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c98b2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c98b2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c98b2-111">Not Supported.</span></span>                         |
| <span data-ttu-id="c98b2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c98b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c98b2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c98b2-113">Not Supported.</span></span>                         |
| <span data-ttu-id="c98b2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c98b2-114">Application</span></span>                            | <span data-ttu-id="c98b2-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c98b2-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="c98b2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c98b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /communications/calls/{id}
```
> <span data-ttu-id="c98b2-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="c98b2-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="c98b2-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="c98b2-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c98b2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c98b2-119">Request headers</span></span>
| <span data-ttu-id="c98b2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c98b2-120">Name</span></span>          | <span data-ttu-id="c98b2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c98b2-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c98b2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c98b2-122">Authorization</span></span> | <span data-ttu-id="c98b2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c98b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c98b2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c98b2-125">Request body</span></span>
<span data-ttu-id="c98b2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c98b2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c98b2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c98b2-127">Response</span></span>
<span data-ttu-id="c98b2-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c98b2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c98b2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c98b2-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c98b2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c98b2-131">Request</span></span>
<span data-ttu-id="c98b2-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c98b2-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c98b2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c98b2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[<span data-ttu-id="c98b2-134">C#</span><span class="sxs-lookup"><span data-stu-id="c98b2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c98b2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c98b2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c98b2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c98b2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c98b2-137">Java</span><span class="sxs-lookup"><span data-stu-id="c98b2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c98b2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c98b2-138">Response</span></span>

> <span data-ttu-id="c98b2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c98b2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="c98b2-141">Notificação - término</span><span class="sxs-lookup"><span data-stu-id="c98b2-141">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="c98b2-142">Notificação - encerrada</span><span class="sxs-lookup"><span data-stu-id="c98b2-142">Notification - terminated</span></span>

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



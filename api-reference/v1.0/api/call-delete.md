---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 708ff1466b86be842e751c3a79cf17dbf1ad64bd
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913601"
---
# <a name="delete-call"></a><span data-ttu-id="8ccd7-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="8ccd7-103">Delete call</span></span>

<span data-ttu-id="8ccd7-104">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-104">Delete or hang up an active call.</span></span> <span data-ttu-id="8ccd7-105">Para chamadas de grupo, isso só excluirá o trecho de chamada, e a chamada de grupo subjacente ainda continuará.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-105">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ccd7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ccd7-106">Permissions</span></span>

| <span data-ttu-id="8ccd7-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ccd7-107">Permission type</span></span> | <span data-ttu-id="8ccd7-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ccd7-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="8ccd7-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ccd7-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ccd7-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-110">Not Supported.</span></span>                         |
| <span data-ttu-id="8ccd7-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ccd7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ccd7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-112">Not Supported.</span></span>                         |
| <span data-ttu-id="8ccd7-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ccd7-113">Application</span></span>                            | <span data-ttu-id="8ccd7-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-114">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8ccd7-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ccd7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ccd7-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ccd7-116">Request headers</span></span>
| <span data-ttu-id="8ccd7-117">Nome</span><span class="sxs-lookup"><span data-stu-id="8ccd7-117">Name</span></span>          | <span data-ttu-id="8ccd7-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ccd7-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8ccd7-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ccd7-119">Authorization</span></span> | <span data-ttu-id="8ccd7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ccd7-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ccd7-122">Request body</span></span>
<span data-ttu-id="8ccd7-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ccd7-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ccd7-124">Response</span></span>
<span data-ttu-id="8ccd7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ccd7-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ccd7-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8ccd7-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ccd7-128">Request</span></span>
<span data-ttu-id="8ccd7-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-129">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ccd7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ccd7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ccd7-131">C#</span><span class="sxs-lookup"><span data-stu-id="8ccd7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ccd7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ccd7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ccd7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ccd7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ccd7-134">Java</span><span class="sxs-lookup"><span data-stu-id="8ccd7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ccd7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ccd7-135">Response</span></span>

> <span data-ttu-id="8ccd7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ccd7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="8ccd7-138">Notificação-encerramento</span><span class="sxs-lookup"><span data-stu-id="8ccd7-138">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="8ccd7-139">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="8ccd7-139">Notification - terminated</span></span>

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

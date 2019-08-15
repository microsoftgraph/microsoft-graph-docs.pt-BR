---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cfc0578261d4821bd4992b3a066c83194e40d1f1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418976"
---
# <a name="delete-call"></a><span data-ttu-id="f8145-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="f8145-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8145-104">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="f8145-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8145-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8145-105">Permissions</span></span>

<span data-ttu-id="f8145-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8145-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8145-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8145-108">Permission type</span></span> | <span data-ttu-id="f8145-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8145-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f8145-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8145-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8145-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8145-111">Not Supported.</span></span>                         |
| <span data-ttu-id="f8145-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8145-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8145-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8145-113">Not Supported.</span></span>                         |
| <span data-ttu-id="f8145-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8145-114">Application</span></span>                            | <span data-ttu-id="f8145-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8145-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="f8145-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8145-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f8145-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8145-117">Request headers</span></span>
| <span data-ttu-id="f8145-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f8145-118">Name</span></span>          | <span data-ttu-id="f8145-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8145-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f8145-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8145-120">Authorization</span></span> | <span data-ttu-id="f8145-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8145-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8145-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8145-123">Request body</span></span>
<span data-ttu-id="f8145-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8145-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8145-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8145-125">Response</span></span>
<span data-ttu-id="f8145-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8145-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8145-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8145-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f8145-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8145-129">Request</span></span>
<span data-ttu-id="f8145-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8145-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f8145-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8145-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8145-132">C#</span><span class="sxs-lookup"><span data-stu-id="f8145-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8145-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8145-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8145-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f8145-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f8145-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8145-135">Response</span></span>

> <span data-ttu-id="f8145-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8145-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="f8145-138">Notificação-encerramento</span><span class="sxs-lookup"><span data-stu-id="f8145-138">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="f8145-139">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="f8145-139">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
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

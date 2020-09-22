---
title: Excluir indicador de inteligência de ameaças
description: Excluir um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b5de10f7423294b0e9d0a044c6a8fcd7b0c831d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994362"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="f938e-103">Excluir indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="f938e-103">Delete threat intelligence indicator</span></span>

<span data-ttu-id="f938e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f938e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f938e-105">Excluir um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="f938e-105">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f938e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f938e-106">Permissions</span></span>

<span data-ttu-id="f938e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f938e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f938e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f938e-109">Permission type</span></span>                        | <span data-ttu-id="f938e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f938e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f938e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f938e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f938e-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f938e-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="f938e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f938e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f938e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f938e-114">Not supported.</span></span> |
| <span data-ttu-id="f938e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f938e-115">Application</span></span>                            | <span data-ttu-id="f938e-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f938e-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="f938e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f938e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f938e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f938e-118">Request headers</span></span>

| <span data-ttu-id="f938e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f938e-119">Name</span></span>          | <span data-ttu-id="f938e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f938e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f938e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f938e-121">Authorization</span></span> | <span data-ttu-id="f938e-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f938e-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f938e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f938e-123">Request body</span></span>

<span data-ttu-id="f938e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f938e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f938e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f938e-125">Response</span></span>

<span data-ttu-id="f938e-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f938e-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f938e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f938e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f938e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f938e-129">Request</span></span>

<span data-ttu-id="f938e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f938e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f938e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f938e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="f938e-132">C#</span><span class="sxs-lookup"><span data-stu-id="f938e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f938e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f938e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f938e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f938e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f938e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f938e-135">Response</span></span>

<span data-ttu-id="f938e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f938e-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



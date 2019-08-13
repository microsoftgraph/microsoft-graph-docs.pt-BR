---
title: Excluir indicador de inteligência de ameaças
description: Excluir um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 790509aa9cc74dcd13ebcbed68e0e5816d6d0566
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362784"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="e5929-103">Excluir indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="e5929-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5929-104">Excluir um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="e5929-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5929-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5929-105">Permissions</span></span>

<span data-ttu-id="e5929-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5929-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5929-108">Permission type</span></span>                        | <span data-ttu-id="e5929-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5929-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5929-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5929-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5929-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e5929-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e5929-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5929-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5929-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5929-113">Not supported.</span></span> |
| <span data-ttu-id="e5929-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5929-114">Application</span></span>                            | <span data-ttu-id="e5929-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e5929-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5929-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5929-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e5929-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5929-117">Request headers</span></span>

| <span data-ttu-id="e5929-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e5929-118">Name</span></span>          | <span data-ttu-id="e5929-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5929-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e5929-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5929-120">Authorization</span></span> | <span data-ttu-id="e5929-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e5929-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5929-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5929-122">Request body</span></span>

<span data-ttu-id="e5929-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5929-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5929-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5929-124">Response</span></span>

<span data-ttu-id="e5929-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5929-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5929-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5929-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5929-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5929-128">Request</span></span>

<span data-ttu-id="e5929-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5929-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e5929-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5929-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5929-131">C#</span><span class="sxs-lookup"><span data-stu-id="e5929-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5929-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5929-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5929-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e5929-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e5929-134">Java</span><span class="sxs-lookup"><span data-stu-id="e5929-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5929-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5929-135">Response</span></span>

<span data-ttu-id="e5929-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5929-136">The following is an example of the response.</span></span>

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

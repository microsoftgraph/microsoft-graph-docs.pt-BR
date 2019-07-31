---
title: Excluir indicador de inteligência de ameaças
description: Excluir um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: e29999ad47c1252762fd4b1c9c243ba2f9f68d93
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987926"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="90b85-103">Excluir indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="90b85-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90b85-104">Excluir um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="90b85-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90b85-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="90b85-105">Permissions</span></span>

<span data-ttu-id="90b85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90b85-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90b85-108">Permission type</span></span>                        | <span data-ttu-id="90b85-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90b85-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90b85-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90b85-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="90b85-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="90b85-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="90b85-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90b85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b85-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90b85-113">Not supported.</span></span> |
| <span data-ttu-id="90b85-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90b85-114">Application</span></span>                            | <span data-ttu-id="90b85-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="90b85-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="90b85-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90b85-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90b85-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90b85-117">Request headers</span></span>

| <span data-ttu-id="90b85-118">Nome</span><span class="sxs-lookup"><span data-stu-id="90b85-118">Name</span></span>          | <span data-ttu-id="90b85-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="90b85-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="90b85-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="90b85-120">Authorization</span></span> | <span data-ttu-id="90b85-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="90b85-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="90b85-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90b85-122">Request body</span></span>

<span data-ttu-id="90b85-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90b85-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90b85-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b85-124">Response</span></span>

<span data-ttu-id="90b85-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90b85-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90b85-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90b85-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90b85-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90b85-128">Request</span></span>

<span data-ttu-id="90b85-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90b85-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90b85-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="90b85-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90b85-131">C#</span><span class="sxs-lookup"><span data-stu-id="90b85-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90b85-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="90b85-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90b85-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="90b85-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="90b85-134">Java</span><span class="sxs-lookup"><span data-stu-id="90b85-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90b85-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b85-135">Response</span></span>

<span data-ttu-id="90b85-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90b85-136">The following is an example of the response.</span></span>

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

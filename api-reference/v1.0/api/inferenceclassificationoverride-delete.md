---
title: Excluir inferenceClassificationOverride
description: Exclua uma substituição especificada de acordo com sua ID.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: df8a850a220c8f1d60329b4adfc658e9eaad9bf9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050448"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="105df-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="105df-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="105df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="105df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="105df-105">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="105df-105">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="105df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="105df-106">Permissions</span></span>
<span data-ttu-id="105df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="105df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="105df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="105df-109">Permission type</span></span>      | <span data-ttu-id="105df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="105df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="105df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="105df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="105df-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="105df-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="105df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="105df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="105df-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="105df-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="105df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="105df-115">Application</span></span> | <span data-ttu-id="105df-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="105df-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="105df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="105df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="105df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="105df-118">Request headers</span></span>
| <span data-ttu-id="105df-119">Nome</span><span class="sxs-lookup"><span data-stu-id="105df-119">Name</span></span>       | <span data-ttu-id="105df-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="105df-120">Type</span></span> | <span data-ttu-id="105df-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="105df-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="105df-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="105df-122">Authorization</span></span>  | <span data-ttu-id="105df-123">string</span><span class="sxs-lookup"><span data-stu-id="105df-123">string</span></span>  | <span data-ttu-id="105df-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="105df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="105df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="105df-126">Request body</span></span>
<span data-ttu-id="105df-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="105df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="105df-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="105df-128">Response</span></span>

<span data-ttu-id="105df-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="105df-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="105df-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="105df-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="105df-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="105df-132">Request</span></span>
<span data-ttu-id="105df-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="105df-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="105df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="105df-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="105df-135">C#</span><span class="sxs-lookup"><span data-stu-id="105df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="105df-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="105df-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="105df-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="105df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="105df-138">Java</span><span class="sxs-lookup"><span data-stu-id="105df-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="105df-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="105df-139">Response</span></span>
<span data-ttu-id="105df-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="105df-140">Here is an example of the response.</span></span> <span data-ttu-id="105df-141">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="105df-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


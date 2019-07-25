---
title: Excluir inferenceClassificationOverride
description: Exclua uma substituição especificada de acordo com sua ID.
localization_priority: Normal
ms.openlocfilehash: f65c95ec40672335d4a9eae330ae1ba080030405
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880814"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="5dbe3-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="5dbe3-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="5dbe3-104">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="5dbe3-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="5dbe3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dbe3-105">Permissions</span></span>
<span data-ttu-id="5dbe3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dbe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dbe3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dbe3-108">Permission type</span></span>      | <span data-ttu-id="5dbe3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dbe3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dbe3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dbe3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5dbe3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dbe3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5dbe3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dbe3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dbe3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dbe3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5dbe3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dbe3-114">Application</span></span> | <span data-ttu-id="5dbe3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dbe3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dbe3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dbe3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5dbe3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dbe3-117">Request headers</span></span>
| <span data-ttu-id="5dbe3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5dbe3-118">Name</span></span>       | <span data-ttu-id="5dbe3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dbe3-119">Type</span></span> | <span data-ttu-id="5dbe3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dbe3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5dbe3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dbe3-121">Authorization</span></span>  | <span data-ttu-id="5dbe3-122">string</span><span class="sxs-lookup"><span data-stu-id="5dbe3-122">string</span></span>  | <span data-ttu-id="5dbe3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dbe3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dbe3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dbe3-125">Request body</span></span>
<span data-ttu-id="5dbe3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5dbe3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dbe3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dbe3-127">Response</span></span>

<span data-ttu-id="5dbe3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dbe3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dbe3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dbe3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dbe3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dbe3-131">Request</span></span>
<span data-ttu-id="5dbe3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dbe3-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5dbe3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dbe3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5dbe3-134">C#</span><span class="sxs-lookup"><span data-stu-id="5dbe3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dbe3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="5dbe3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5dbe3-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5dbe3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5dbe3-137">Java</span><span class="sxs-lookup"><span data-stu-id="5dbe3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5dbe3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dbe3-138">Response</span></span>
<span data-ttu-id="5dbe3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dbe3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

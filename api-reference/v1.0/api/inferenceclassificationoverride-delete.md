---
title: Excluir inferenceClassificationOverride
description: Exclua uma substituição especificada de acordo com sua ID.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 62b5d76219e34afc5200ea9c8f8fcaddbca4714e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516728"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="23f76-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="23f76-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="23f76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23f76-105">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="23f76-105">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="23f76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23f76-106">Permissions</span></span>
<span data-ttu-id="23f76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23f76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23f76-109">Permission type</span></span>      | <span data-ttu-id="23f76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23f76-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23f76-111">Delegated (work or school account)</span></span> | <span data-ttu-id="23f76-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23f76-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="23f76-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23f76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f76-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23f76-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="23f76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23f76-115">Application</span></span> | <span data-ttu-id="23f76-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23f76-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23f76-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="23f76-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23f76-118">Request headers</span></span>
| <span data-ttu-id="23f76-119">Nome</span><span class="sxs-lookup"><span data-stu-id="23f76-119">Name</span></span>       | <span data-ttu-id="23f76-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="23f76-120">Type</span></span> | <span data-ttu-id="23f76-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f76-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23f76-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23f76-122">Authorization</span></span>  | <span data-ttu-id="23f76-123">string</span><span class="sxs-lookup"><span data-stu-id="23f76-123">string</span></span>  | <span data-ttu-id="23f76-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23f76-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23f76-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23f76-126">Request body</span></span>
<span data-ttu-id="23f76-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23f76-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f76-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f76-128">Response</span></span>

<span data-ttu-id="23f76-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23f76-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23f76-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23f76-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23f76-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23f76-132">Request</span></span>
<span data-ttu-id="23f76-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23f76-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23f76-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f76-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="23f76-135">C#</span><span class="sxs-lookup"><span data-stu-id="23f76-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23f76-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23f76-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23f76-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23f76-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23f76-138">Java</span><span class="sxs-lookup"><span data-stu-id="23f76-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23f76-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f76-139">Response</span></span>
<span data-ttu-id="23f76-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23f76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

---
title: Excluir contrato
description: Exclua um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: e954c23f6fb44b6258f468808370dc73a4af440c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962482"
---
# <a name="delete-agreement"></a><span data-ttu-id="9ad2b-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="9ad2b-103">Delete agreement</span></span>

<span data-ttu-id="9ad2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ad2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ad2b-105">Exclua um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="9ad2b-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ad2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ad2b-106">Permissions</span></span>
<span data-ttu-id="9ad2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ad2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ad2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ad2b-109">Permission type</span></span>                        | <span data-ttu-id="9ad2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ad2b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ad2b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ad2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ad2b-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad2b-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="9ad2b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ad2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad2b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad2b-114">Not supported.</span></span> |
|<span data-ttu-id="9ad2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ad2b-115">Application</span></span>                            | <span data-ttu-id="9ad2b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad2b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ad2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ad2b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9ad2b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad2b-118">Request headers</span></span>
| <span data-ttu-id="9ad2b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9ad2b-119">Name</span></span>         | <span data-ttu-id="9ad2b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ad2b-120">Type</span></span>        | <span data-ttu-id="9ad2b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ad2b-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ad2b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ad2b-122">Authorization</span></span> | <span data-ttu-id="9ad2b-123">string</span><span class="sxs-lookup"><span data-stu-id="9ad2b-123">string</span></span> | <span data-ttu-id="9ad2b-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ad2b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ad2b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad2b-126">Request body</span></span>
<span data-ttu-id="9ad2b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ad2b-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9ad2b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ad2b-128">Response</span></span>
<span data-ttu-id="9ad2b-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ad2b-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ad2b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ad2b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ad2b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad2b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9ad2b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ad2b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="9ad2b-134">C#</span><span class="sxs-lookup"><span data-stu-id="9ad2b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ad2b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ad2b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ad2b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ad2b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ad2b-137">Java</span><span class="sxs-lookup"><span data-stu-id="9ad2b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9ad2b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ad2b-138">Response</span></span>
><span data-ttu-id="9ad2b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ad2b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



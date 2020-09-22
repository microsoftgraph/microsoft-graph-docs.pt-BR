---
title: Excluir contrato
description: Exclua um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 69bcef2996fff224a5d5839667087d860f4f5b2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997171"
---
# <a name="delete-agreement"></a><span data-ttu-id="c0909-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="c0909-103">Delete agreement</span></span>

<span data-ttu-id="c0909-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0909-105">Exclua um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="c0909-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0909-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0909-106">Permissions</span></span>
<span data-ttu-id="c0909-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0909-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0909-109">Permission type</span></span>                        | <span data-ttu-id="c0909-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0909-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0909-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0909-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0909-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0909-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="c0909-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0909-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0909-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0909-114">Not supported.</span></span> |
|<span data-ttu-id="c0909-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0909-115">Application</span></span>                            | <span data-ttu-id="c0909-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0909-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0909-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0909-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c0909-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0909-118">Request headers</span></span>
| <span data-ttu-id="c0909-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c0909-119">Name</span></span>         | <span data-ttu-id="c0909-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0909-120">Type</span></span>        | <span data-ttu-id="c0909-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0909-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c0909-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0909-122">Authorization</span></span> | <span data-ttu-id="c0909-123">string</span><span class="sxs-lookup"><span data-stu-id="c0909-123">string</span></span> | <span data-ttu-id="c0909-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0909-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0909-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0909-126">Request body</span></span>
<span data-ttu-id="c0909-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0909-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c0909-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0909-128">Response</span></span>
<span data-ttu-id="c0909-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0909-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0909-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0909-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0909-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0909-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0909-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0909-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="c0909-134">C#</span><span class="sxs-lookup"><span data-stu-id="c0909-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0909-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0909-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0909-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0909-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0909-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0909-137">Response</span></span>
><span data-ttu-id="c0909-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0909-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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



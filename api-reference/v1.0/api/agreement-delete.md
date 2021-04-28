---
title: Excluir contrato
description: Excluir um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 3afecd702e5c0e674e301f94cb6f8ec1cd95a8df
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040151"
---
# <a name="delete-agreement"></a><span data-ttu-id="2c79a-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="2c79a-103">Delete agreement</span></span>

<span data-ttu-id="2c79a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c79a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c79a-105">Excluir um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="2c79a-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c79a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c79a-106">Permissions</span></span>
<span data-ttu-id="2c79a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c79a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c79a-109">Permission type</span></span>                        | <span data-ttu-id="2c79a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c79a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c79a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c79a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c79a-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c79a-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="2c79a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c79a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c79a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c79a-114">Not supported.</span></span> |
|<span data-ttu-id="2c79a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c79a-115">Application</span></span>                            | <span data-ttu-id="2c79a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c79a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c79a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c79a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2c79a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c79a-118">Request headers</span></span>
| <span data-ttu-id="2c79a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2c79a-119">Name</span></span>         | <span data-ttu-id="2c79a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c79a-120">Type</span></span>        | <span data-ttu-id="2c79a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c79a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2c79a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c79a-122">Authorization</span></span> | <span data-ttu-id="2c79a-123">string</span><span class="sxs-lookup"><span data-stu-id="2c79a-123">string</span></span> | <span data-ttu-id="2c79a-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c79a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c79a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c79a-126">Request body</span></span>
<span data-ttu-id="2c79a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c79a-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2c79a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c79a-128">Response</span></span>
<span data-ttu-id="2c79a-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c79a-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c79a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c79a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2c79a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c79a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2c79a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c79a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be
```
# <a name="c"></a>[<span data-ttu-id="2c79a-134">C#</span><span class="sxs-lookup"><span data-stu-id="2c79a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c79a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c79a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c79a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c79a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c79a-137">Java</span><span class="sxs-lookup"><span data-stu-id="2c79a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c79a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c79a-138">Response</span></span>
><span data-ttu-id="2c79a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2c79a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



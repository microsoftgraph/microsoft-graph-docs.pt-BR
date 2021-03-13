---
title: Excluir contrato
description: Excluir um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: b9b441be1d3b8af2b79a4a71425059d90ba3cc37
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768907"
---
# <a name="delete-agreement"></a><span data-ttu-id="f1284-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="f1284-103">Delete agreement</span></span>

<span data-ttu-id="f1284-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1284-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1284-105">Excluir um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="f1284-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1284-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1284-106">Permissions</span></span>
<span data-ttu-id="f1284-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1284-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1284-109">Permission type</span></span>                        | <span data-ttu-id="f1284-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1284-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1284-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1284-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1284-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1284-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="f1284-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1284-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1284-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1284-114">Not supported.</span></span> |
|<span data-ttu-id="f1284-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1284-115">Application</span></span>                            | <span data-ttu-id="f1284-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1284-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1284-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1284-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f1284-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1284-118">Request headers</span></span>
| <span data-ttu-id="f1284-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f1284-119">Name</span></span>         | <span data-ttu-id="f1284-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1284-120">Type</span></span>        | <span data-ttu-id="f1284-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1284-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f1284-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1284-122">Authorization</span></span> | <span data-ttu-id="f1284-123">string</span><span class="sxs-lookup"><span data-stu-id="f1284-123">string</span></span> | <span data-ttu-id="f1284-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1284-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1284-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1284-126">Request body</span></span>
<span data-ttu-id="f1284-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1284-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f1284-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1284-128">Response</span></span>
<span data-ttu-id="f1284-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1284-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1284-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1284-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1284-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1284-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f1284-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1284-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be
```
# <a name="c"></a>[<span data-ttu-id="f1284-134">C#</span><span class="sxs-lookup"><span data-stu-id="f1284-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1284-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1284-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1284-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1284-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1284-137">Java</span><span class="sxs-lookup"><span data-stu-id="f1284-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1284-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1284-138">Response</span></span>
><span data-ttu-id="f1284-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1284-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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



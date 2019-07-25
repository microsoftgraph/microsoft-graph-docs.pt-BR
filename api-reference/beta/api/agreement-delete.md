---
title: Excluir contrato
description: Exclua um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 2b0bf56bf63a62cacd757035f10f0cbb48a30604
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855515"
---
# <a name="delete-agreement"></a><span data-ttu-id="a7998-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="a7998-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7998-104">Exclua um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="a7998-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7998-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7998-105">Permissions</span></span>
<span data-ttu-id="a7998-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7998-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7998-108">Permission type</span></span>                        | <span data-ttu-id="a7998-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7998-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7998-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7998-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7998-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7998-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="a7998-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7998-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7998-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7998-113">Not supported.</span></span> |
|<span data-ttu-id="a7998-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7998-114">Application</span></span>                            | <span data-ttu-id="a7998-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7998-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7998-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7998-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="a7998-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7998-117">Request headers</span></span>
| <span data-ttu-id="a7998-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a7998-118">Name</span></span>         | <span data-ttu-id="a7998-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7998-119">Type</span></span>        | <span data-ttu-id="a7998-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7998-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a7998-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7998-121">Authorization</span></span> | <span data-ttu-id="a7998-122">string</span><span class="sxs-lookup"><span data-stu-id="a7998-122">string</span></span> | <span data-ttu-id="a7998-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7998-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7998-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7998-125">Request body</span></span>
<span data-ttu-id="a7998-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7998-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a7998-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7998-127">Response</span></span>
<span data-ttu-id="a7998-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7998-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7998-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7998-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7998-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7998-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7998-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7998-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7998-133">C#</span><span class="sxs-lookup"><span data-stu-id="a7998-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7998-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7998-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7998-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a7998-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7998-136">Java</span><span class="sxs-lookup"><span data-stu-id="a7998-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7998-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7998-137">Response</span></span>
><span data-ttu-id="a7998-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7998-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

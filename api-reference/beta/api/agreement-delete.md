---
title: Excluir contrato
description: Exclua um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 4b7e10567c658799c97f881026de812f3b510162
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439830"
---
# <a name="delete-agreement"></a><span data-ttu-id="cbb14-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="cbb14-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbb14-104">Exclua um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="cbb14-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbb14-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbb14-105">Permissions</span></span>
<span data-ttu-id="cbb14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbb14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbb14-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbb14-108">Permission type</span></span>                        | <span data-ttu-id="cbb14-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbb14-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbb14-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbb14-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbb14-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb14-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="cbb14-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbb14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbb14-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbb14-113">Not supported.</span></span> |
|<span data-ttu-id="cbb14-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbb14-114">Application</span></span>                            | <span data-ttu-id="cbb14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbb14-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbb14-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbb14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="cbb14-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbb14-117">Request headers</span></span>
| <span data-ttu-id="cbb14-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cbb14-118">Name</span></span>         | <span data-ttu-id="cbb14-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbb14-119">Type</span></span>        | <span data-ttu-id="cbb14-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbb14-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cbb14-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbb14-121">Authorization</span></span> | <span data-ttu-id="cbb14-122">string</span><span class="sxs-lookup"><span data-stu-id="cbb14-122">string</span></span> | <span data-ttu-id="cbb14-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbb14-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbb14-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbb14-125">Request body</span></span>
<span data-ttu-id="cbb14-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbb14-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cbb14-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbb14-127">Response</span></span>
<span data-ttu-id="cbb14-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbb14-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbb14-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbb14-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbb14-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbb14-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cbb14-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbb14-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbb14-133">C#</span><span class="sxs-lookup"><span data-stu-id="cbb14-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbb14-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbb14-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbb14-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cbb14-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cbb14-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbb14-136">Response</span></span>
><span data-ttu-id="cbb14-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbb14-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

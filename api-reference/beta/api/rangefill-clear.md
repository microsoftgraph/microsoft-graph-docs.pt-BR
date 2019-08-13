---
title: 'RangeFill: clear'
description: Redefine o plano de fundo do intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d171258f4af97bd5edb5b286b1277bfd4a6e40cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360730"
---
# <a name="rangefill-clear"></a><span data-ttu-id="47a83-103">RangeFill: clear</span><span class="sxs-lookup"><span data-stu-id="47a83-103">RangeFill: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47a83-104">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="47a83-104">Resets the range background.</span></span>
## <a name="permissions"></a><span data-ttu-id="47a83-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47a83-105">Permissions</span></span>
<span data-ttu-id="47a83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47a83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a83-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47a83-108">Permission type</span></span>      | <span data-ttu-id="47a83-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47a83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a83-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47a83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47a83-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47a83-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="47a83-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47a83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47a83-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47a83-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="47a83-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47a83-114">Application</span></span> | <span data-ttu-id="47a83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47a83-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47a83-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47a83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/fill/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="47a83-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47a83-117">Request headers</span></span>
| <span data-ttu-id="47a83-118">Nome</span><span class="sxs-lookup"><span data-stu-id="47a83-118">Name</span></span>       | <span data-ttu-id="47a83-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="47a83-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47a83-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="47a83-120">Authorization</span></span>  | <span data-ttu-id="47a83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47a83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47a83-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47a83-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="47a83-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="47a83-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47a83-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47a83-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="47a83-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a83-127">Response</span></span>

<span data-ttu-id="47a83-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a83-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47a83-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47a83-130">Example</span></span>
<span data-ttu-id="47a83-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="47a83-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47a83-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47a83-132">Request</span></span>
<span data-ttu-id="47a83-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47a83-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47a83-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="47a83-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangefill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47a83-135">C#</span><span class="sxs-lookup"><span data-stu-id="47a83-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangefill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47a83-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47a83-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangefill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47a83-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="47a83-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangefill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="47a83-138">Java</span><span class="sxs-lookup"><span data-stu-id="47a83-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangefill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="47a83-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a83-139">Response</span></span>
<span data-ttu-id="47a83-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a83-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

---
title: 'ChartFill: setSolidColor'
description: Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9249e0517754d18407682d9f52c82e480fc9fcda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943943"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="59d08-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="59d08-103">ChartFill: setSolidColor</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59d08-104">Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.</span><span class="sxs-lookup"><span data-stu-id="59d08-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="59d08-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="59d08-105">Permissions</span></span>
<span data-ttu-id="59d08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59d08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59d08-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59d08-108">Permission type</span></span>      | <span data-ttu-id="59d08-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59d08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59d08-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59d08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59d08-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d08-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59d08-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59d08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d08-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d08-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59d08-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59d08-114">Application</span></span> | <span data-ttu-id="59d08-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59d08-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59d08-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59d08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="59d08-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59d08-117">Request headers</span></span>
| <span data-ttu-id="59d08-118">Nome</span><span class="sxs-lookup"><span data-stu-id="59d08-118">Name</span></span>       | <span data-ttu-id="59d08-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d08-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59d08-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="59d08-120">Authorization</span></span>  | <span data-ttu-id="59d08-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59d08-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59d08-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59d08-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="59d08-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="59d08-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59d08-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59d08-126">Request body</span></span>
<span data-ttu-id="59d08-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d08-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59d08-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59d08-128">Parameter</span></span>    | <span data-ttu-id="59d08-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="59d08-129">Type</span></span>   |<span data-ttu-id="59d08-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d08-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d08-131">color</span><span class="sxs-lookup"><span data-stu-id="59d08-131">color</span></span>|<span data-ttu-id="59d08-132">string</span><span class="sxs-lookup"><span data-stu-id="59d08-132">string</span></span>|<span data-ttu-id="59d08-133">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="59d08-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="59d08-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d08-134">Response</span></span>

<span data-ttu-id="59d08-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d08-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59d08-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59d08-137">Example</span></span>
<span data-ttu-id="59d08-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="59d08-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59d08-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59d08-139">Request</span></span>
<span data-ttu-id="59d08-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d08-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59d08-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="59d08-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59d08-142">C#</span><span class="sxs-lookup"><span data-stu-id="59d08-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59d08-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="59d08-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59d08-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="59d08-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59d08-145">Java</span><span class="sxs-lookup"><span data-stu-id="59d08-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59d08-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d08-146">Response</span></span>
<span data-ttu-id="59d08-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d08-147">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

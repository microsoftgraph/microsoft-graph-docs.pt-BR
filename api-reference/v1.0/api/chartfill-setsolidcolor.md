---
title: 'ChartFill: setSolidColor'
description: Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c44580e0a91977c5251b43d5c8d812a127690b44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059828"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="874b5-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="874b5-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="874b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="874b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="874b5-105">Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.</span><span class="sxs-lookup"><span data-stu-id="874b5-105">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="874b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="874b5-106">Permissions</span></span>
<span data-ttu-id="874b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874b5-109">Permission type</span></span>      | <span data-ttu-id="874b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="874b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="874b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="874b5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="874b5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="874b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="874b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874b5-114">Not supported.</span></span>    |
|<span data-ttu-id="874b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="874b5-115">Application</span></span> | <span data-ttu-id="874b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874b5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="874b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="874b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874b5-118">Request headers</span></span>
| <span data-ttu-id="874b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="874b5-119">Name</span></span>       | <span data-ttu-id="874b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="874b5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="874b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="874b5-121">Authorization</span></span>  | <span data-ttu-id="874b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="874b5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="874b5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="874b5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="874b5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="874b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874b5-127">Request body</span></span>
<span data-ttu-id="874b5-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874b5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="874b5-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="874b5-129">Parameter</span></span>    | <span data-ttu-id="874b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="874b5-130">Type</span></span>   |<span data-ttu-id="874b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="874b5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="874b5-132">color</span><span class="sxs-lookup"><span data-stu-id="874b5-132">color</span></span>|<span data-ttu-id="874b5-133">string</span><span class="sxs-lookup"><span data-stu-id="874b5-133">string</span></span>|<span data-ttu-id="874b5-134">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="874b5-134">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="874b5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="874b5-135">Response</span></span>

<span data-ttu-id="874b5-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874b5-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="874b5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="874b5-138">Example</span></span>
<span data-ttu-id="874b5-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="874b5-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="874b5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874b5-140">Request</span></span>
<span data-ttu-id="874b5-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874b5-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="874b5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="874b5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="874b5-143">C#</span><span class="sxs-lookup"><span data-stu-id="874b5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="874b5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="874b5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="874b5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="874b5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="874b5-146">Java</span><span class="sxs-lookup"><span data-stu-id="874b5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="874b5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="874b5-147">Response</span></span>
<span data-ttu-id="874b5-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874b5-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


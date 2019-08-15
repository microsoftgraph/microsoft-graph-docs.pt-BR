---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8a2e0d8910e0933c86c8a4112c41a5ab53253383
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421338"
---
# <a name="tablesort-apply"></a><span data-ttu-id="0c66c-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="0c66c-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c66c-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="0c66c-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c66c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c66c-105">Permissions</span></span>
<span data-ttu-id="0c66c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c66c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c66c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c66c-108">Permission type</span></span>      | <span data-ttu-id="0c66c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c66c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c66c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c66c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c66c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c66c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c66c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c66c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c66c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c66c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c66c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c66c-114">Application</span></span> | <span data-ttu-id="0c66c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c66c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c66c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c66c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="0c66c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c66c-117">Request headers</span></span>
| <span data-ttu-id="0c66c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0c66c-118">Name</span></span>       | <span data-ttu-id="0c66c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c66c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c66c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c66c-120">Authorization</span></span>  | <span data-ttu-id="0c66c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c66c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c66c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0c66c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0c66c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0c66c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c66c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c66c-126">Request body</span></span>
<span data-ttu-id="0c66c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c66c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c66c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0c66c-128">Parameter</span></span>    | <span data-ttu-id="0c66c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c66c-129">Type</span></span>   |<span data-ttu-id="0c66c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c66c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c66c-131">campos</span><span class="sxs-lookup"><span data-stu-id="0c66c-131">fields</span></span>|<span data-ttu-id="0c66c-132">coleção workbookSortField</span><span class="sxs-lookup"><span data-stu-id="0c66c-132">workbookSortField collection</span></span>|<span data-ttu-id="0c66c-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="0c66c-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="0c66c-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="0c66c-134">matchCase</span></span>|<span data-ttu-id="0c66c-135">booliano</span><span class="sxs-lookup"><span data-stu-id="0c66c-135">boolean</span></span>|<span data-ttu-id="0c66c-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="0c66c-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="0c66c-138">method</span><span class="sxs-lookup"><span data-stu-id="0c66c-138">method</span></span>|<span data-ttu-id="0c66c-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c66c-139">string</span></span>|<span data-ttu-id="0c66c-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="0c66c-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="0c66c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c66c-143">Response</span></span>

<span data-ttu-id="0c66c-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c66c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c66c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c66c-146">Example</span></span>
<span data-ttu-id="0c66c-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0c66c-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c66c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c66c-148">Request</span></span>
<span data-ttu-id="0c66c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c66c-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c66c-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c66c-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c66c-151">C#</span><span class="sxs-lookup"><span data-stu-id="0c66c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c66c-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c66c-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c66c-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0c66c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c66c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c66c-154">Response</span></span>
<span data-ttu-id="0c66c-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c66c-155">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

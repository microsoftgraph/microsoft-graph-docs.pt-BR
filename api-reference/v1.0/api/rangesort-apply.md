---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bd71fd26d7a81e09ca73a5393c6532ff3d5c842
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275436"
---
# <a name="rangesort-apply"></a><span data-ttu-id="d6216-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="d6216-103">RangeSort: apply</span></span>

<span data-ttu-id="d6216-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="d6216-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6216-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6216-105">Permissions</span></span>
<span data-ttu-id="d6216-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6216-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6216-108">Permission type</span></span>      | <span data-ttu-id="d6216-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6216-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6216-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6216-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6216-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6216-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6216-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6216-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6216-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6216-113">Not supported.</span></span>    |
|<span data-ttu-id="d6216-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6216-114">Application</span></span> | <span data-ttu-id="d6216-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6216-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6216-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6216-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="d6216-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6216-117">Request headers</span></span>
| <span data-ttu-id="d6216-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d6216-118">Name</span></span>       | <span data-ttu-id="d6216-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6216-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d6216-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6216-120">Authorization</span></span>  | <span data-ttu-id="d6216-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6216-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6216-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d6216-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d6216-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6216-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6216-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6216-126">Request body</span></span>
<span data-ttu-id="d6216-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6216-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d6216-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d6216-128">Parameter</span></span>    | <span data-ttu-id="d6216-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6216-129">Type</span></span>   |<span data-ttu-id="d6216-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6216-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6216-131">campos</span><span class="sxs-lookup"><span data-stu-id="d6216-131">fields</span></span>|<span data-ttu-id="d6216-132">Coleção WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="d6216-132">WorkbookSortField collection</span></span>|<span data-ttu-id="d6216-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="d6216-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="d6216-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="d6216-134">matchCase</span></span>|<span data-ttu-id="d6216-135">booliano</span><span class="sxs-lookup"><span data-stu-id="d6216-135">boolean</span></span>|<span data-ttu-id="d6216-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d6216-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="d6216-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="d6216-138">hasHeaders</span></span>|<span data-ttu-id="d6216-139">booliano</span><span class="sxs-lookup"><span data-stu-id="d6216-139">boolean</span></span>|<span data-ttu-id="d6216-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="d6216-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="d6216-142">orientation</span><span class="sxs-lookup"><span data-stu-id="d6216-142">orientation</span></span>|<span data-ttu-id="d6216-143">string</span><span class="sxs-lookup"><span data-stu-id="d6216-143">string</span></span>|<span data-ttu-id="d6216-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6216-144">Optional.</span></span> <span data-ttu-id="d6216-145">Se a operação classifica linhas ou colunas.</span><span class="sxs-lookup"><span data-stu-id="d6216-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="d6216-146">Os valores possíveis são: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="d6216-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="d6216-147">method</span><span class="sxs-lookup"><span data-stu-id="d6216-147">method</span></span>|<span data-ttu-id="d6216-148">string</span><span class="sxs-lookup"><span data-stu-id="d6216-148">string</span></span>|<span data-ttu-id="d6216-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6216-149">Optional.</span></span> <span data-ttu-id="d6216-150">O método de ordenação usado pelos caracteres chineses.</span><span class="sxs-lookup"><span data-stu-id="d6216-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="d6216-151">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="d6216-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="d6216-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6216-152">Response</span></span>

<span data-ttu-id="d6216-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6216-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6216-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6216-155">Example</span></span>
<span data-ttu-id="d6216-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d6216-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d6216-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6216-157">Request</span></span>
<span data-ttu-id="d6216-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6216-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="d6216-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6216-159">Response</span></span>
<span data-ttu-id="d6216-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6216-160">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6216-161">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d6216-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6216-162">C#</span><span class="sxs-lookup"><span data-stu-id="d6216-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/rangesort_apply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6216-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6216-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangesort_apply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d6216-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d6216-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/rangesort_apply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangesort-apply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangesort-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangesort-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

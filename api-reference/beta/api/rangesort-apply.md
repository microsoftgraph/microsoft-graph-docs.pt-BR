---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a81c799df7a1f161bfa1718e32d72ad9f415cdf3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981130"
---
# <a name="rangesort-apply"></a><span data-ttu-id="dee6f-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="dee6f-103">RangeSort: apply</span></span>

<span data-ttu-id="dee6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dee6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dee6f-105">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="dee6f-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="dee6f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dee6f-106">Permissions</span></span>
<span data-ttu-id="dee6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee6f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dee6f-109">Permission type</span></span>      | <span data-ttu-id="dee6f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dee6f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dee6f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dee6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dee6f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dee6f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dee6f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dee6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dee6f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dee6f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dee6f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dee6f-115">Application</span></span> | <span data-ttu-id="dee6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dee6f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dee6f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dee6f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="dee6f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dee6f-118">Request headers</span></span>
| <span data-ttu-id="dee6f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dee6f-119">Name</span></span>       | <span data-ttu-id="dee6f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dee6f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dee6f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dee6f-121">Authorization</span></span>  | <span data-ttu-id="dee6f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dee6f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dee6f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dee6f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dee6f-127">Request body</span></span>
<span data-ttu-id="dee6f-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dee6f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dee6f-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dee6f-129">Parameter</span></span>    | <span data-ttu-id="dee6f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dee6f-130">Type</span></span>   |<span data-ttu-id="dee6f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dee6f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dee6f-132">campos</span><span class="sxs-lookup"><span data-stu-id="dee6f-132">fields</span></span>|<span data-ttu-id="dee6f-133">coleção workbookSortField</span><span class="sxs-lookup"><span data-stu-id="dee6f-133">workbookSortField collection</span></span>|<span data-ttu-id="dee6f-134">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="dee6f-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="dee6f-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="dee6f-135">matchCase</span></span>|<span data-ttu-id="dee6f-136">booliano</span><span class="sxs-lookup"><span data-stu-id="dee6f-136">boolean</span></span>|<span data-ttu-id="dee6f-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="dee6f-139">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="dee6f-139">hasHeaders</span></span>|<span data-ttu-id="dee6f-140">booliano</span><span class="sxs-lookup"><span data-stu-id="dee6f-140">boolean</span></span>|<span data-ttu-id="dee6f-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="dee6f-143">orientation</span><span class="sxs-lookup"><span data-stu-id="dee6f-143">orientation</span></span>|<span data-ttu-id="dee6f-144">string</span><span class="sxs-lookup"><span data-stu-id="dee6f-144">string</span></span>|<span data-ttu-id="dee6f-p106">Opcional. Se a operação classifica linhas ou colunas.  Os valores possíveis são: `Rows` e `Columns`.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="dee6f-148">método</span><span class="sxs-lookup"><span data-stu-id="dee6f-148">method</span></span>|<span data-ttu-id="dee6f-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dee6f-149">string</span></span>|<span data-ttu-id="dee6f-p107">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="dee6f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="dee6f-153">Response</span></span>

<span data-ttu-id="dee6f-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dee6f-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dee6f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dee6f-156">Example</span></span>
<span data-ttu-id="dee6f-157">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dee6f-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dee6f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dee6f-158">Request</span></span>
<span data-ttu-id="dee6f-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dee6f-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dee6f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="dee6f-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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
# <a name="c"></a>[<span data-ttu-id="dee6f-161">C#</span><span class="sxs-lookup"><span data-stu-id="dee6f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dee6f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dee6f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dee6f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dee6f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dee6f-164">Java</span><span class="sxs-lookup"><span data-stu-id="dee6f-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dee6f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="dee6f-165">Response</span></span>
<span data-ttu-id="dee6f-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dee6f-166">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



---
title: 'RangeSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b95bc4c8aeda5463304c2fd8d5fd26d565eb7f16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510463"
---
# <a name="rangesort-apply"></a><span data-ttu-id="d02fd-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="d02fd-103">RangeSort: apply</span></span>

<span data-ttu-id="d02fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d02fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d02fd-105">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="d02fd-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="d02fd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d02fd-106">Permissions</span></span>
<span data-ttu-id="d02fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d02fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d02fd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d02fd-109">Permission type</span></span>      | <span data-ttu-id="d02fd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d02fd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d02fd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d02fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d02fd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d02fd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d02fd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d02fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d02fd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d02fd-114">Not supported.</span></span>    |
|<span data-ttu-id="d02fd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d02fd-115">Application</span></span> | <span data-ttu-id="d02fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d02fd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d02fd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d02fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="d02fd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d02fd-118">Request headers</span></span>
| <span data-ttu-id="d02fd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d02fd-119">Name</span></span>       | <span data-ttu-id="d02fd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d02fd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d02fd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d02fd-121">Authorization</span></span>  | <span data-ttu-id="d02fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d02fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d02fd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d02fd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d02fd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d02fd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d02fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d02fd-127">Request body</span></span>
<span data-ttu-id="d02fd-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d02fd-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d02fd-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d02fd-129">Parameter</span></span>    | <span data-ttu-id="d02fd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d02fd-130">Type</span></span>   |<span data-ttu-id="d02fd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d02fd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d02fd-132">campos</span><span class="sxs-lookup"><span data-stu-id="d02fd-132">fields</span></span>|<span data-ttu-id="d02fd-133">Coleção WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="d02fd-133">WorkbookSortField collection</span></span>|<span data-ttu-id="d02fd-134">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="d02fd-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="d02fd-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="d02fd-135">matchCase</span></span>|<span data-ttu-id="d02fd-136">booliano</span><span class="sxs-lookup"><span data-stu-id="d02fd-136">boolean</span></span>|<span data-ttu-id="d02fd-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d02fd-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="d02fd-139">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="d02fd-139">hasHeaders</span></span>|<span data-ttu-id="d02fd-140">booliano</span><span class="sxs-lookup"><span data-stu-id="d02fd-140">boolean</span></span>|<span data-ttu-id="d02fd-p105">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="d02fd-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="d02fd-143">orientation</span><span class="sxs-lookup"><span data-stu-id="d02fd-143">orientation</span></span>|<span data-ttu-id="d02fd-144">string</span><span class="sxs-lookup"><span data-stu-id="d02fd-144">string</span></span>|<span data-ttu-id="d02fd-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d02fd-145">Optional.</span></span> <span data-ttu-id="d02fd-146">Se a operação classifica linhas ou colunas.</span><span class="sxs-lookup"><span data-stu-id="d02fd-146">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="d02fd-147">Os valores possíveis são: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="d02fd-147">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="d02fd-148">method</span><span class="sxs-lookup"><span data-stu-id="d02fd-148">method</span></span>|<span data-ttu-id="d02fd-149">string</span><span class="sxs-lookup"><span data-stu-id="d02fd-149">string</span></span>|<span data-ttu-id="d02fd-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d02fd-150">Optional.</span></span> <span data-ttu-id="d02fd-151">O método de ordenação usado pelos caracteres chineses.</span><span class="sxs-lookup"><span data-stu-id="d02fd-151">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="d02fd-152">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="d02fd-152">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="d02fd-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d02fd-153">Response</span></span>

<span data-ttu-id="d02fd-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d02fd-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d02fd-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d02fd-156">Example</span></span>
<span data-ttu-id="d02fd-157">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d02fd-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d02fd-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d02fd-158">Request</span></span>
<span data-ttu-id="d02fd-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d02fd-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d02fd-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d02fd-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d02fd-161">C#</span><span class="sxs-lookup"><span data-stu-id="d02fd-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d02fd-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d02fd-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d02fd-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d02fd-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d02fd-164">Java</span><span class="sxs-lookup"><span data-stu-id="d02fd-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d02fd-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d02fd-165">Response</span></span>
<span data-ttu-id="d02fd-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d02fd-166">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

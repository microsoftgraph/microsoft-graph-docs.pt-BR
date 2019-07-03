---
title: 'workbookRange: rowsBelow'
description: Obtém um determinado número de linhas abaixo de um determinado intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b51bb7fbe40e4c2f1316b42a96fcd4631864db54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458744"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="f9cf2-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="f9cf2-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="f9cf2-104">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9cf2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9cf2-105">Permissions</span></span>
<span data-ttu-id="f9cf2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9cf2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9cf2-108">Permission type</span></span>      | <span data-ttu-id="f9cf2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9cf2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9cf2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9cf2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9cf2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9cf2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9cf2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9cf2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9cf2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-113">Not supported.</span></span>    |
|<span data-ttu-id="f9cf2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9cf2-114">Application</span></span> | <span data-ttu-id="f9cf2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9cf2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cf2-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9cf2-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cf2-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="f9cf2-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f9cf2-118">Function parameters</span></span>

| <span data-ttu-id="f9cf2-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9cf2-119">Parameter</span></span>    | <span data-ttu-id="f9cf2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9cf2-120">Type</span></span>   |<span data-ttu-id="f9cf2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9cf2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9cf2-122">Count</span><span class="sxs-lookup"><span data-stu-id="f9cf2-122">count</span></span>|<span data-ttu-id="f9cf2-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f9cf2-123">Int32</span></span>| <span data-ttu-id="f9cf2-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f9cf2-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf2-129">Request headers</span></span>
| <span data-ttu-id="f9cf2-130">Nome</span><span class="sxs-lookup"><span data-stu-id="f9cf2-130">Name</span></span>       | <span data-ttu-id="f9cf2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9cf2-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9cf2-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9cf2-132">Authorization</span></span>  | <span data-ttu-id="f9cf2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9cf2-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9cf2-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9cf2-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9cf2-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf2-138">Request body</span></span>
<span data-ttu-id="f9cf2-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9cf2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cf2-140">Response</span></span>
<span data-ttu-id="f9cf2-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9cf2-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9cf2-142">Example</span></span>
<span data-ttu-id="f9cf2-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9cf2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf2-144">Request</span></span>
<span data-ttu-id="f9cf2-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9cf2-146">C#</span><span class="sxs-lookup"><span data-stu-id="f9cf2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9cf2-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9cf2-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9cf2-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f9cf2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9cf2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cf2-149">Response</span></span>
<span data-ttu-id="f9cf2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9cf2-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cf2-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<span data-ttu-id="f9cf2-154">Se chamado sem o `count` parâmetro, essa função será padronizada como uma linha.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-154">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="f9cf2-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf2-155">Request</span></span>
<span data-ttu-id="f9cf2-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-156">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9cf2-157">C#</span><span class="sxs-lookup"><span data-stu-id="f9cf2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9cf2-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9cf2-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9cf2-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f9cf2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9cf2-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cf2-160">Response</span></span>
<span data-ttu-id="f9cf2-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9cf2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

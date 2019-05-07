---
title: 'workbookRange: rowsAbove'
description: Obtém um determinado número de linhas acima de um determinado intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 05d860d9fa5e022dc4978f6f734ae149964e4404
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601007"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="f29cc-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="f29cc-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="f29cc-104">Obtém um determinado número de linhas acima de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="f29cc-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f29cc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f29cc-105">Permissions</span></span>
<span data-ttu-id="f29cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f29cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f29cc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f29cc-108">Permission type</span></span>      | <span data-ttu-id="f29cc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f29cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f29cc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f29cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f29cc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29cc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f29cc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f29cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f29cc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f29cc-113">Not supported.</span></span>    |
|<span data-ttu-id="f29cc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f29cc-114">Application</span></span> | <span data-ttu-id="f29cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f29cc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f29cc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f29cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="f29cc-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f29cc-117">Function parameters</span></span>

| <span data-ttu-id="f29cc-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f29cc-118">Parameter</span></span>    | <span data-ttu-id="f29cc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f29cc-119">Type</span></span>   |<span data-ttu-id="f29cc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f29cc-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f29cc-121">Count</span><span class="sxs-lookup"><span data-stu-id="f29cc-121">count</span></span>|<span data-ttu-id="f29cc-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f29cc-122">Int32</span></span>|<span data-ttu-id="f29cc-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="f29cc-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f29cc-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f29cc-128">Request headers</span></span>
| <span data-ttu-id="f29cc-129">Nome</span><span class="sxs-lookup"><span data-stu-id="f29cc-129">Name</span></span>       | <span data-ttu-id="f29cc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f29cc-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f29cc-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f29cc-131">Authorization</span></span>  | <span data-ttu-id="f29cc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f29cc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f29cc-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f29cc-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="f29cc-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f29cc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f29cc-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f29cc-137">Request body</span></span>
<span data-ttu-id="f29cc-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f29cc-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f29cc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29cc-139">Response</span></span>
<span data-ttu-id="f29cc-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f29cc-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f29cc-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f29cc-141">Example</span></span>
<span data-ttu-id="f29cc-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f29cc-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f29cc-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f29cc-143">Request</span></span>
<span data-ttu-id="f29cc-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f29cc-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="f29cc-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29cc-145">Response</span></span>
<span data-ttu-id="f29cc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f29cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f29cc-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f29cc-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f29cc-150">Basic</span><span class="sxs-lookup"><span data-stu-id="f29cc-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f29cc-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f29cc-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f29cc-152">Se chamado sem o parâmetro `count` opcional, essa função retornará a única linha acima do intervalo.</span><span class="sxs-lookup"><span data-stu-id="f29cc-152">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="f29cc-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f29cc-153">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="f29cc-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29cc-154">Response</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f29cc-155">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f29cc-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f29cc-156">Basic</span><span class="sxs-lookup"><span data-stu-id="f29cc-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove_nocount-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f29cc-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f29cc-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove_nocount-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

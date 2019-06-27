---
title: 'workbookRange: columnsAfter'
description: Obtém um determinado número de colunas à direita do intervalo especificado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dd9ea54b31952fa297128ca3ac6e2a80552bc921
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269374"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="8d841-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="8d841-103">workbookRange: columnsAfter</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d841-104">Obtém um determinado número de colunas à direita do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="8d841-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d841-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d841-105">Permissions</span></span>
<span data-ttu-id="8d841-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d841-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d841-108">Permission type</span></span>      | <span data-ttu-id="8d841-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d841-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d841-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d841-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d841-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d841-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d841-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d841-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d841-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d841-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d841-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d841-114">Application</span></span> | <span data-ttu-id="8d841-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d841-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d841-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d841-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="8d841-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8d841-117">Function parameters</span></span>

| <span data-ttu-id="8d841-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d841-118">Parameter</span></span>    | <span data-ttu-id="8d841-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d841-119">Type</span></span>   |<span data-ttu-id="8d841-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d841-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d841-121">Count</span><span class="sxs-lookup"><span data-stu-id="8d841-121">count</span></span>|<span data-ttu-id="8d841-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8d841-122">Int32</span></span>|<span data-ttu-id="8d841-p102">O número de colunas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="8d841-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8d841-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d841-127">Request headers</span></span>
| <span data-ttu-id="8d841-128">Nome</span><span class="sxs-lookup"><span data-stu-id="8d841-128">Name</span></span>       | <span data-ttu-id="8d841-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d841-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d841-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d841-130">Authorization</span></span>  | <span data-ttu-id="8d841-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d841-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d841-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8d841-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d841-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8d841-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d841-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d841-136">Request body</span></span>
<span data-ttu-id="8d841-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d841-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d841-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d841-138">Response</span></span>

<span data-ttu-id="8d841-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d841-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d841-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d841-140">Example</span></span>
<span data-ttu-id="8d841-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8d841-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d841-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d841-142">Request</span></span>
<span data-ttu-id="8d841-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d841-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="8d841-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d841-144">Response</span></span>
<span data-ttu-id="8d841-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d841-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d841-148">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8d841-148">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d841-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d841-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_columnsafter-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="8d841-150">C#</span><span class="sxs-lookup"><span data-stu-id="8d841-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_columnsafter-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8d841-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8d841-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_columnsafter-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

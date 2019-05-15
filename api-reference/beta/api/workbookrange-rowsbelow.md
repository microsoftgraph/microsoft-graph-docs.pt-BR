---
title: 'workbookRange: rowsBelow'
description: Obtém um determinado número de linhas abaixo de um determinado intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e2818704f8a6aa6b186c8f5e04445ec46b4e2017
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961079"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="fc2ca-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="fc2ca-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc2ca-104">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc2ca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc2ca-105">Permissions</span></span>
<span data-ttu-id="fc2ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc2ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc2ca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc2ca-108">Permission type</span></span>      | <span data-ttu-id="fc2ca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc2ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc2ca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc2ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc2ca-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc2ca-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc2ca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc2ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc2ca-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc2ca-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc2ca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc2ca-114">Application</span></span> | <span data-ttu-id="fc2ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc2ca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc2ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="fc2ca-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="fc2ca-117">Function parameters</span></span>

| <span data-ttu-id="fc2ca-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fc2ca-118">Parameter</span></span>    | <span data-ttu-id="fc2ca-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc2ca-119">Type</span></span>   |<span data-ttu-id="fc2ca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc2ca-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc2ca-121">Count</span><span class="sxs-lookup"><span data-stu-id="fc2ca-121">count</span></span>|<span data-ttu-id="fc2ca-122">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2ca-122">Int32</span></span>|<span data-ttu-id="fc2ca-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fc2ca-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc2ca-128">Request headers</span></span>
| <span data-ttu-id="fc2ca-129">Nome</span><span class="sxs-lookup"><span data-stu-id="fc2ca-129">Name</span></span>       | <span data-ttu-id="fc2ca-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc2ca-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc2ca-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc2ca-131">Authorization</span></span>  | <span data-ttu-id="fc2ca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc2ca-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc2ca-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc2ca-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc2ca-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc2ca-137">Request body</span></span>
<span data-ttu-id="fc2ca-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc2ca-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc2ca-139">Response</span></span>

<span data-ttu-id="fc2ca-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc2ca-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc2ca-141">Example</span></span>
<span data-ttu-id="fc2ca-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc2ca-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc2ca-143">Request</span></span>
<span data-ttu-id="fc2ca-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="fc2ca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc2ca-145">Response</span></span>
<span data-ttu-id="fc2ca-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc2ca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc2ca-149">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="fc2ca-149">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc2ca-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc2ca-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="fc2ca-151">C#</span><span class="sxs-lookup"><span data-stu-id="fc2ca-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

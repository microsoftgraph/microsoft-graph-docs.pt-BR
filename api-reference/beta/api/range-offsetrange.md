---
title: 'Range: OffsetRange'
description: Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e30c732a6e4595229c693d55647e938e8b13e5c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055068"
---
# <a name="range-offsetrange"></a><span data-ttu-id="305fe-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="305fe-105">Range: OffsetRange</span></span>

<span data-ttu-id="305fe-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="305fe-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="305fe-p102">Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.</span><span class="sxs-lookup"><span data-stu-id="305fe-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="305fe-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="305fe-110">Permissions</span></span>
<span data-ttu-id="305fe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="305fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="305fe-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="305fe-113">Permission type</span></span>      | <span data-ttu-id="305fe-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="305fe-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="305fe-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="305fe-115">Delegated (work or school account)</span></span> | <span data-ttu-id="305fe-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="305fe-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="305fe-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="305fe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="305fe-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="305fe-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="305fe-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="305fe-119">Application</span></span> | <span data-ttu-id="305fe-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="305fe-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="305fe-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="305fe-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/OffsetRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="305fe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="305fe-122">Request headers</span></span>
| <span data-ttu-id="305fe-123">Nome</span><span class="sxs-lookup"><span data-stu-id="305fe-123">Name</span></span>       | <span data-ttu-id="305fe-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="305fe-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="305fe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="305fe-125">Authorization</span></span>  | <span data-ttu-id="305fe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="305fe-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="305fe-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="305fe-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="305fe-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="305fe-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="305fe-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="305fe-131">Request body</span></span>
<span data-ttu-id="305fe-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="305fe-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="305fe-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="305fe-133">Parameter</span></span>    | <span data-ttu-id="305fe-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="305fe-134">Type</span></span>   |<span data-ttu-id="305fe-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="305fe-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="305fe-136">rowOffset</span><span class="sxs-lookup"><span data-stu-id="305fe-136">rowOffset</span></span>|<span data-ttu-id="305fe-137">number</span><span class="sxs-lookup"><span data-stu-id="305fe-137">number</span></span>|<span data-ttu-id="305fe-p106">O número de linhas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para baixo e os negativos, para cima.</span><span class="sxs-lookup"><span data-stu-id="305fe-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="305fe-140">columnOffset</span><span class="sxs-lookup"><span data-stu-id="305fe-140">columnOffset</span></span>|<span data-ttu-id="305fe-141">number</span><span class="sxs-lookup"><span data-stu-id="305fe-141">number</span></span>|<span data-ttu-id="305fe-p107">O número de colunas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para a direita e os negativos, para a esquerda.</span><span class="sxs-lookup"><span data-stu-id="305fe-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="305fe-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="305fe-144">Response</span></span>

<span data-ttu-id="305fe-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="305fe-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="305fe-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="305fe-146">Example</span></span>
<span data-ttu-id="305fe-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="305fe-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="305fe-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="305fe-148">Request</span></span>
<span data-ttu-id="305fe-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="305fe-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="305fe-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="305fe-150">Response</span></span>
<span data-ttu-id="305fe-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="305fe-151">Here is an example of the response.</span></span> <span data-ttu-id="305fe-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="305fe-152">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



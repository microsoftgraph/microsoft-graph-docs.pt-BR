---
title: 'Range: OffsetRange'
description: Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8819c7c2ff8ff07c0206e6b9491e926616f3e1ee
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576194"
---
# <a name="range-offsetrange"></a><span data-ttu-id="85d62-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="85d62-105">Range: OffsetRange</span></span>

<span data-ttu-id="85d62-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d62-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85d62-p102">Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.</span><span class="sxs-lookup"><span data-stu-id="85d62-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="85d62-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="85d62-110">Permissions</span></span>
<span data-ttu-id="85d62-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d62-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d62-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85d62-113">Permission type</span></span>      | <span data-ttu-id="85d62-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85d62-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85d62-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85d62-115">Delegated (work or school account)</span></span> | <span data-ttu-id="85d62-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85d62-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85d62-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85d62-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d62-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85d62-118">Not supported.</span></span>    |
|<span data-ttu-id="85d62-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85d62-119">Application</span></span> | <span data-ttu-id="85d62-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85d62-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85d62-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85d62-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/offsetRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/offsetRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/offsetRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/offsetRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/offsetRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/offsetRange

```
## <a name="request-headers"></a><span data-ttu-id="85d62-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85d62-122">Request headers</span></span>
| <span data-ttu-id="85d62-123">Nome</span><span class="sxs-lookup"><span data-stu-id="85d62-123">Name</span></span>       | <span data-ttu-id="85d62-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="85d62-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="85d62-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="85d62-125">Authorization</span></span>  | <span data-ttu-id="85d62-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85d62-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85d62-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85d62-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="85d62-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="85d62-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d62-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85d62-131">Request body</span></span>
<span data-ttu-id="85d62-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85d62-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85d62-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="85d62-133">Parameter</span></span>    | <span data-ttu-id="85d62-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="85d62-134">Type</span></span>   |<span data-ttu-id="85d62-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="85d62-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85d62-136">rowOffset</span><span class="sxs-lookup"><span data-stu-id="85d62-136">rowOffset</span></span>|<span data-ttu-id="85d62-137">Int32</span><span class="sxs-lookup"><span data-stu-id="85d62-137">Int32</span></span>|<span data-ttu-id="85d62-p106">O número de linhas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para baixo e os negativos, para cima.</span><span class="sxs-lookup"><span data-stu-id="85d62-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="85d62-140">columnOffset</span><span class="sxs-lookup"><span data-stu-id="85d62-140">columnOffset</span></span>|<span data-ttu-id="85d62-141">Int32</span><span class="sxs-lookup"><span data-stu-id="85d62-141">Int32</span></span>|<span data-ttu-id="85d62-p107">O número de colunas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para a direita e os negativos, para a esquerda.</span><span class="sxs-lookup"><span data-stu-id="85d62-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="85d62-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d62-144">Response</span></span>

<span data-ttu-id="85d62-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85d62-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d62-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85d62-146">Example</span></span>
<span data-ttu-id="85d62-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="85d62-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85d62-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85d62-148">Request</span></span>
<span data-ttu-id="85d62-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85d62-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/offsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": 3,
  "columnOffset": 5
}
```

##### <a name="response"></a><span data-ttu-id="85d62-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d62-150">Response</span></span>
<span data-ttu-id="85d62-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85d62-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


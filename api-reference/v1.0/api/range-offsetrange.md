---
title: 'Range: OffsetRange'
description: Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fe1c368eff0c03df0fe454684139720ec8360ac5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025285"
---
# <a name="range-offsetrange"></a><span data-ttu-id="566bc-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="566bc-105">Range: OffsetRange</span></span>

<span data-ttu-id="566bc-p102">Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.</span><span class="sxs-lookup"><span data-stu-id="566bc-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="566bc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="566bc-109">Permissions</span></span>
<span data-ttu-id="566bc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="566bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="566bc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="566bc-112">Permission type</span></span>      | <span data-ttu-id="566bc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="566bc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="566bc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="566bc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="566bc-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="566bc-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="566bc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="566bc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="566bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="566bc-117">Not supported.</span></span>    |
|<span data-ttu-id="566bc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="566bc-118">Application</span></span> | <span data-ttu-id="566bc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="566bc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="566bc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="566bc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/offsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/offsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/offsetRange

```
## <a name="request-headers"></a><span data-ttu-id="566bc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="566bc-121">Request headers</span></span>
| <span data-ttu-id="566bc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="566bc-122">Name</span></span>       | <span data-ttu-id="566bc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="566bc-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="566bc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="566bc-124">Authorization</span></span>  | <span data-ttu-id="566bc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="566bc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="566bc-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="566bc-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="566bc-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="566bc-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="566bc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="566bc-130">Request body</span></span>
<span data-ttu-id="566bc-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="566bc-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="566bc-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="566bc-132">Parameter</span></span>    | <span data-ttu-id="566bc-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="566bc-133">Type</span></span>   |<span data-ttu-id="566bc-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="566bc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="566bc-135">rowOffset</span><span class="sxs-lookup"><span data-stu-id="566bc-135">rowOffset</span></span>|<span data-ttu-id="566bc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="566bc-136">Int32</span></span>|<span data-ttu-id="566bc-p106">O número de linhas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para baixo e os negativos, para cima.</span><span class="sxs-lookup"><span data-stu-id="566bc-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="566bc-139">columnOffset</span><span class="sxs-lookup"><span data-stu-id="566bc-139">columnOffset</span></span>|<span data-ttu-id="566bc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="566bc-140">Int32</span></span>|<span data-ttu-id="566bc-p107">O número de colunas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para a direita e os negativos, para a esquerda.</span><span class="sxs-lookup"><span data-stu-id="566bc-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="566bc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="566bc-143">Response</span></span>

<span data-ttu-id="566bc-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="566bc-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="566bc-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="566bc-145">Example</span></span>
<span data-ttu-id="566bc-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="566bc-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="566bc-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="566bc-147">Request</span></span>
<span data-ttu-id="566bc-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="566bc-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="566bc-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="566bc-149">Response</span></span>
<span data-ttu-id="566bc-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="566bc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

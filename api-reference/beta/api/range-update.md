---
title: Intervalo de atualização
description: Atualize as propriedades do objeto range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eda7a9122884776131a65722c493031ba0bb1098
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643007"
---
# <a name="update-range"></a><span data-ttu-id="1e66a-103">Intervalo de atualização</span><span class="sxs-lookup"><span data-stu-id="1e66a-103">Update range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e66a-104">Atualize as propriedades do objeto range.</span><span class="sxs-lookup"><span data-stu-id="1e66a-104">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e66a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e66a-105">Permissions</span></span>
<span data-ttu-id="1e66a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e66a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e66a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e66a-108">Permission type</span></span>      | <span data-ttu-id="1e66a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e66a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e66a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e66a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e66a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e66a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e66a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e66a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e66a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e66a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e66a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e66a-114">Application</span></span> | <span data-ttu-id="1e66a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e66a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e66a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e66a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="1e66a-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1e66a-117">Optional request headers</span></span>
| <span data-ttu-id="1e66a-118">Name</span><span class="sxs-lookup"><span data-stu-id="1e66a-118">Name</span></span>       | <span data-ttu-id="1e66a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e66a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1e66a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e66a-120">Authorization</span></span>  | <span data-ttu-id="1e66a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e66a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1e66a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e66a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e66a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e66a-126">Request body</span></span>
<span data-ttu-id="1e66a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e66a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e66a-130">Property</span></span>     | <span data-ttu-id="1e66a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e66a-131">Type</span></span>   |<span data-ttu-id="1e66a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e66a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e66a-133">columnHidden</span><span class="sxs-lookup"><span data-stu-id="1e66a-133">columnHidden</span></span>|<span data-ttu-id="1e66a-134">booliano</span><span class="sxs-lookup"><span data-stu-id="1e66a-134">boolean</span></span>|<span data-ttu-id="1e66a-135">Representa se todas as colunas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="1e66a-135">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="1e66a-136">fórmulas</span><span class="sxs-lookup"><span data-stu-id="1e66a-136">formulas</span></span>|<span data-ttu-id="1e66a-137">json</span><span class="sxs-lookup"><span data-stu-id="1e66a-137">json</span></span>|<span data-ttu-id="1e66a-138">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="1e66a-138">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="1e66a-139">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="1e66a-139">formulasLocal</span></span>|<span data-ttu-id="1e66a-140">json</span><span class="sxs-lookup"><span data-stu-id="1e66a-140">json</span></span>|<span data-ttu-id="1e66a-p105">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="1e66a-143">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="1e66a-143">formulasR1C1</span></span>|<span data-ttu-id="1e66a-144">json</span><span class="sxs-lookup"><span data-stu-id="1e66a-144">json</span></span>|<span data-ttu-id="1e66a-145">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="1e66a-145">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="1e66a-146">numberFormat</span><span class="sxs-lookup"><span data-stu-id="1e66a-146">numberFormat</span></span>|<span data-ttu-id="1e66a-147">json</span><span class="sxs-lookup"><span data-stu-id="1e66a-147">json</span></span>|<span data-ttu-id="1e66a-148">Representa o código de formato de número do Excel para determinada célula.</span><span class="sxs-lookup"><span data-stu-id="1e66a-148">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="1e66a-149">rowHidden</span><span class="sxs-lookup"><span data-stu-id="1e66a-149">rowHidden</span></span>|<span data-ttu-id="1e66a-150">booliano</span><span class="sxs-lookup"><span data-stu-id="1e66a-150">boolean</span></span>|<span data-ttu-id="1e66a-151">Representa se todas as linhas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="1e66a-151">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="1e66a-152">values</span><span class="sxs-lookup"><span data-stu-id="1e66a-152">values</span></span>|<span data-ttu-id="1e66a-153">json</span><span class="sxs-lookup"><span data-stu-id="1e66a-153">json</span></span>|<span data-ttu-id="1e66a-p106">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="1e66a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e66a-157">Response</span></span>

<span data-ttu-id="1e66a-158">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Range](../resources/range.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e66a-158">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e66a-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e66a-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e66a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e66a-160">Request</span></span>
<span data-ttu-id="1e66a-p107">Este é um exemplo da solicitação. Atualiza um intervalo: valores, formato de número e fórmula. A entrada `null` é para instruir a API a ignorar a célula para esta entrada específica. Os valores, o formato de número e as fórmulas podem ser atualizados independentemente ou combinados na mesma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="1e66a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e66a-165">Response</span></span>
<span data-ttu-id="1e66a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e66a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

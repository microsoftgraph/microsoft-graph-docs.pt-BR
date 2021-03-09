---
title: Intervalo de atualização
description: Atualize as propriedades do objeto range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 50f6d99cec55a5d0fd60f941bc2c64c2a6d3e0af
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576689"
---
# <a name="update-range"></a><span data-ttu-id="ce48e-103">Intervalo de atualização</span><span class="sxs-lookup"><span data-stu-id="ce48e-103">Update range</span></span>

<span data-ttu-id="ce48e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce48e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce48e-105">Atualize as propriedades do objeto range.</span><span class="sxs-lookup"><span data-stu-id="ce48e-105">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce48e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce48e-106">Permissions</span></span>
<span data-ttu-id="ce48e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce48e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce48e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce48e-109">Permission type</span></span>      | <span data-ttu-id="ce48e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce48e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce48e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce48e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ce48e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce48e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ce48e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce48e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce48e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce48e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ce48e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce48e-115">Application</span></span> | <span data-ttu-id="ce48e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce48e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce48e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce48e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="ce48e-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ce48e-118">Optional request headers</span></span>
| <span data-ttu-id="ce48e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ce48e-119">Name</span></span>       | <span data-ttu-id="ce48e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce48e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ce48e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce48e-121">Authorization</span></span>  | <span data-ttu-id="ce48e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce48e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ce48e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ce48e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce48e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce48e-127">Request body</span></span>
<span data-ttu-id="ce48e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ce48e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce48e-131">Property</span></span>     | <span data-ttu-id="ce48e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce48e-132">Type</span></span>   |<span data-ttu-id="ce48e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce48e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce48e-134">columnHidden</span><span class="sxs-lookup"><span data-stu-id="ce48e-134">columnHidden</span></span>|<span data-ttu-id="ce48e-135">booliano</span><span class="sxs-lookup"><span data-stu-id="ce48e-135">boolean</span></span>|<span data-ttu-id="ce48e-136">Representa se todas as colunas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="ce48e-136">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="ce48e-137">fórmulas</span><span class="sxs-lookup"><span data-stu-id="ce48e-137">formulas</span></span>|<span data-ttu-id="ce48e-138">Json</span><span class="sxs-lookup"><span data-stu-id="ce48e-138">Json</span></span>|<span data-ttu-id="ce48e-139">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="ce48e-139">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="ce48e-140">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="ce48e-140">formulasLocal</span></span>|<span data-ttu-id="ce48e-141">Json</span><span class="sxs-lookup"><span data-stu-id="ce48e-141">Json</span></span>|<span data-ttu-id="ce48e-p105">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="ce48e-144">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="ce48e-144">formulasR1C1</span></span>|<span data-ttu-id="ce48e-145">Json</span><span class="sxs-lookup"><span data-stu-id="ce48e-145">Json</span></span>|<span data-ttu-id="ce48e-146">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="ce48e-146">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="ce48e-147">numberFormat</span><span class="sxs-lookup"><span data-stu-id="ce48e-147">numberFormat</span></span>|<span data-ttu-id="ce48e-148">Json</span><span class="sxs-lookup"><span data-stu-id="ce48e-148">Json</span></span>|<span data-ttu-id="ce48e-149">Representa o código de formato de número do Excel para determinada célula.</span><span class="sxs-lookup"><span data-stu-id="ce48e-149">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="ce48e-150">rowHidden</span><span class="sxs-lookup"><span data-stu-id="ce48e-150">rowHidden</span></span>|<span data-ttu-id="ce48e-151">booliano</span><span class="sxs-lookup"><span data-stu-id="ce48e-151">boolean</span></span>|<span data-ttu-id="ce48e-152">Representa se todas as linhas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="ce48e-152">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="ce48e-153">values</span><span class="sxs-lookup"><span data-stu-id="ce48e-153">values</span></span>|<span data-ttu-id="ce48e-154">Json</span><span class="sxs-lookup"><span data-stu-id="ce48e-154">Json</span></span>|<span data-ttu-id="ce48e-p106">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="ce48e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce48e-158">Response</span></span>

<span data-ttu-id="ce48e-159">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workbookRange](../resources/workbookrange.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce48e-159">If successful, this method returns a `200 OK` response code and updated [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce48e-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce48e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce48e-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce48e-161">Request</span></span>
<span data-ttu-id="ce48e-p107">Este é um exemplo da solicitação. Atualiza um intervalo: valores, formato de número e fórmula. A entrada `null` é para instruir a API a ignorar a célula para esta entrada específica. Os valores, o formato de número e as fórmulas podem ser atualizados independentemente ou combinados na mesma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 


# <a name="http"></a>[<span data-ttu-id="ce48e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce48e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/sheet1/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formulas" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
# <a name="javascript"></a>[<span data-ttu-id="ce48e-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce48e-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ce48e-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce48e-168">Response</span></span>
<span data-ttu-id="ce48e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce48e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



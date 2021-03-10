---
title: Intervalo de atualização
description: Atualize as propriedades do objeto range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: db1f708d1ddf1e7e9c1b5410133855b136eb4240
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576152"
---
# <a name="update-range"></a><span data-ttu-id="166b5-103">Intervalo de atualização</span><span class="sxs-lookup"><span data-stu-id="166b5-103">Update range</span></span>

<span data-ttu-id="166b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="166b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="166b5-105">Atualize as propriedades do objeto range.</span><span class="sxs-lookup"><span data-stu-id="166b5-105">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="166b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="166b5-106">Permissions</span></span>
<span data-ttu-id="166b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="166b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="166b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="166b5-109">Permission type</span></span>      | <span data-ttu-id="166b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="166b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="166b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="166b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="166b5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="166b5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="166b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="166b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="166b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="166b5-114">Not supported.</span></span>    |
|<span data-ttu-id="166b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="166b5-115">Application</span></span> | <span data-ttu-id="166b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="166b5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="166b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="166b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="166b5-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="166b5-118">Optional request headers</span></span>
| <span data-ttu-id="166b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="166b5-119">Name</span></span>       | <span data-ttu-id="166b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="166b5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="166b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="166b5-121">Authorization</span></span>  | <span data-ttu-id="166b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="166b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="166b5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="166b5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="166b5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="166b5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="166b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="166b5-127">Request body</span></span>
<span data-ttu-id="166b5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="166b5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="166b5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="166b5-131">Property</span></span>     | <span data-ttu-id="166b5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="166b5-132">Type</span></span>   |<span data-ttu-id="166b5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="166b5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="166b5-134">columnHidden</span><span class="sxs-lookup"><span data-stu-id="166b5-134">columnHidden</span></span>|<span data-ttu-id="166b5-135">booliano</span><span class="sxs-lookup"><span data-stu-id="166b5-135">boolean</span></span>|<span data-ttu-id="166b5-136">Representa se todas as colunas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="166b5-136">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="166b5-137">fórmulas</span><span class="sxs-lookup"><span data-stu-id="166b5-137">formulas</span></span>|<span data-ttu-id="166b5-138">Json</span><span class="sxs-lookup"><span data-stu-id="166b5-138">Json</span></span>|<span data-ttu-id="166b5-139">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="166b5-139">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="166b5-140">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="166b5-140">formulasLocal</span></span>|<span data-ttu-id="166b5-141">Json</span><span class="sxs-lookup"><span data-stu-id="166b5-141">Json</span></span>|<span data-ttu-id="166b5-p105">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="166b5-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="166b5-144">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="166b5-144">formulasR1C1</span></span>|<span data-ttu-id="166b5-145">Json</span><span class="sxs-lookup"><span data-stu-id="166b5-145">Json</span></span>|<span data-ttu-id="166b5-146">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="166b5-146">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="166b5-147">numberFormat</span><span class="sxs-lookup"><span data-stu-id="166b5-147">numberFormat</span></span>|<span data-ttu-id="166b5-148">Json</span><span class="sxs-lookup"><span data-stu-id="166b5-148">Json</span></span>|<span data-ttu-id="166b5-149">Representa o código de formato de número do Excel para determinada célula.</span><span class="sxs-lookup"><span data-stu-id="166b5-149">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="166b5-150">rowHidden</span><span class="sxs-lookup"><span data-stu-id="166b5-150">rowHidden</span></span>|<span data-ttu-id="166b5-151">booliano</span><span class="sxs-lookup"><span data-stu-id="166b5-151">boolean</span></span>|<span data-ttu-id="166b5-152">Representa se todas as linhas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="166b5-152">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="166b5-153">values</span><span class="sxs-lookup"><span data-stu-id="166b5-153">values</span></span>|<span data-ttu-id="166b5-154">Json</span><span class="sxs-lookup"><span data-stu-id="166b5-154">Json</span></span>|<span data-ttu-id="166b5-p106">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="166b5-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="166b5-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="166b5-158">Response</span></span>

<span data-ttu-id="166b5-159">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Range](../resources/range.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="166b5-159">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="166b5-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="166b5-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="166b5-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="166b5-161">Request</span></span>
<span data-ttu-id="166b5-p107">Este é um exemplo da solicitação. Atualiza um intervalo: valores, formato de número e fórmula. A entrada `null` é para instruir a API a ignorar a célula para esta entrada específica. Os valores, o formato de número e as fórmulas podem ser atualizados independentemente ou combinados na mesma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="166b5-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 


# <a name="http"></a>[<span data-ttu-id="166b5-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="166b5-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formulas" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
# <a name="javascript"></a>[<span data-ttu-id="166b5-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="166b5-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="166b5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="166b5-168">Response</span></span>
<span data-ttu-id="166b5-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="166b5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->


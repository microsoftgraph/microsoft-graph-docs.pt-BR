# <a name="update-range"></a><span data-ttu-id="7db77-101">Intervalo de atualização</span><span class="sxs-lookup"><span data-stu-id="7db77-101">Update range</span></span>

<span data-ttu-id="7db77-102">Atualize as propriedades do objeto range.</span><span class="sxs-lookup"><span data-stu-id="7db77-102">Update the properties of range object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7db77-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7db77-103">Prerequisites</span></span>
<span data-ttu-id="7db77-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="7db77-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="7db77-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7db77-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="7db77-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7db77-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address=<range-address>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="7db77-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7db77-107">Optional request headers</span></span>
| <span data-ttu-id="7db77-108">Nome</span><span class="sxs-lookup"><span data-stu-id="7db77-108">Name</span></span>       | <span data-ttu-id="7db77-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7db77-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7db77-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="7db77-110">Authorization</span></span>  | <span data-ttu-id="7db77-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7db77-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="7db77-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7db77-113">Request body</span></span>
<span data-ttu-id="7db77-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7db77-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7db77-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7db77-117">Property</span></span>     | <span data-ttu-id="7db77-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="7db77-118">Type</span></span>   |<span data-ttu-id="7db77-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7db77-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7db77-120">columnHidden</span><span class="sxs-lookup"><span data-stu-id="7db77-120">columnHidden</span></span>|<span data-ttu-id="7db77-121">booliano</span><span class="sxs-lookup"><span data-stu-id="7db77-121">boolean</span></span>|<span data-ttu-id="7db77-122">Representa se todas as colunas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="7db77-122">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="7db77-123">fórmulas</span><span class="sxs-lookup"><span data-stu-id="7db77-123">formulas</span></span>|<span data-ttu-id="7db77-124">json</span><span class="sxs-lookup"><span data-stu-id="7db77-124">json</span></span>|<span data-ttu-id="7db77-125">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="7db77-125">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="7db77-126">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="7db77-126">formulasLocal</span></span>|<span data-ttu-id="7db77-127">json</span><span class="sxs-lookup"><span data-stu-id="7db77-127">json</span></span>|<span data-ttu-id="7db77-p103">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="7db77-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="7db77-130">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="7db77-130">formulasR1C1</span></span>|<span data-ttu-id="7db77-131">json</span><span class="sxs-lookup"><span data-stu-id="7db77-131">json</span></span>|<span data-ttu-id="7db77-132">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="7db77-132">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="7db77-133">numberFormat</span><span class="sxs-lookup"><span data-stu-id="7db77-133">numberFormat</span></span>|<span data-ttu-id="7db77-134">json</span><span class="sxs-lookup"><span data-stu-id="7db77-134">json</span></span>|<span data-ttu-id="7db77-135">Representa o código de formato de número do Excel para determinada célula.</span><span class="sxs-lookup"><span data-stu-id="7db77-135">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="7db77-136">rowHidden</span><span class="sxs-lookup"><span data-stu-id="7db77-136">rowHidden</span></span>|<span data-ttu-id="7db77-137">booliano</span><span class="sxs-lookup"><span data-stu-id="7db77-137">boolean</span></span>|<span data-ttu-id="7db77-138">Representa se todas as linhas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="7db77-138">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="7db77-139">values</span><span class="sxs-lookup"><span data-stu-id="7db77-139">values</span></span>|<span data-ttu-id="7db77-140">json</span><span class="sxs-lookup"><span data-stu-id="7db77-140">json</span></span>|<span data-ttu-id="7db77-p104">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="7db77-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="7db77-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db77-144">Response</span></span>

<span data-ttu-id="7db77-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Range](../resources/range.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7db77-145">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7db77-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7db77-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7db77-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7db77-147">Request</span></span>
<span data-ttu-id="7db77-p105">Este é um exemplo da solicitação. Atualiza um intervalo: valores, formato de número e fórmula. A entrada `null` é para instruir a API a ignorar a célula para esta entrada específica. Os valores, o formato de número e as fórmulas podem ser atualizados independentemente ou combinados na mesma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="7db77-p105">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="7db77-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db77-152">Response</span></span>
<span data-ttu-id="7db77-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7db77-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

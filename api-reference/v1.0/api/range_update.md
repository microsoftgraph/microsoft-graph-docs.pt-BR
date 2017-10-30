# <a name="update-range"></a><span data-ttu-id="21b44-101">Intervalo de atualização</span><span class="sxs-lookup"><span data-stu-id="21b44-101">Update range</span></span>

<span data-ttu-id="21b44-102">Atualize as propriedades do objeto range.</span><span class="sxs-lookup"><span data-stu-id="21b44-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="21b44-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="21b44-103">Permissions</span></span>
<span data-ttu-id="21b44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="21b44-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21b44-106">Permission type</span></span>      | <span data-ttu-id="21b44-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21b44-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21b44-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21b44-108">Delegated (work or school account)</span></span> | <span data-ttu-id="21b44-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21b44-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21b44-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21b44-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21b44-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21b44-111">Not supported.</span></span>    |
|<span data-ttu-id="21b44-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21b44-112">Application</span></span> | <span data-ttu-id="21b44-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21b44-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21b44-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21b44-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="21b44-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="21b44-115">Optional request headers</span></span>
| <span data-ttu-id="21b44-116">Nome</span><span class="sxs-lookup"><span data-stu-id="21b44-116">Name</span></span>       | <span data-ttu-id="21b44-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b44-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="21b44-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="21b44-118">Authorization</span></span>  | <span data-ttu-id="21b44-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21b44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21b44-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21b44-121">Request body</span></span>
<span data-ttu-id="21b44-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="21b44-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="21b44-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21b44-125">Property</span></span>     | <span data-ttu-id="21b44-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b44-126">Type</span></span>   |<span data-ttu-id="21b44-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b44-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b44-128">columnHidden</span><span class="sxs-lookup"><span data-stu-id="21b44-128">columnHidden</span></span>|<span data-ttu-id="21b44-129">booliano</span><span class="sxs-lookup"><span data-stu-id="21b44-129">boolean</span></span>|<span data-ttu-id="21b44-130">Representa se todas as colunas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="21b44-130">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="21b44-131">fórmulas</span><span class="sxs-lookup"><span data-stu-id="21b44-131">formulas</span></span>|<span data-ttu-id="21b44-132">json</span><span class="sxs-lookup"><span data-stu-id="21b44-132">json</span></span>|<span data-ttu-id="21b44-133">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="21b44-133">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="21b44-134">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="21b44-134">formulasLocal</span></span>|<span data-ttu-id="21b44-135">json</span><span class="sxs-lookup"><span data-stu-id="21b44-135">json</span></span>|<span data-ttu-id="21b44-p104">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="21b44-p104">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="21b44-138">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="21b44-138">formulasR1C1</span></span>|<span data-ttu-id="21b44-139">json</span><span class="sxs-lookup"><span data-stu-id="21b44-139">json</span></span>|<span data-ttu-id="21b44-140">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="21b44-140">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="21b44-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="21b44-141">numberFormat</span></span>|<span data-ttu-id="21b44-142">json</span><span class="sxs-lookup"><span data-stu-id="21b44-142">json</span></span>|<span data-ttu-id="21b44-143">Representa o código de formato de número do Excel para determinada célula.</span><span class="sxs-lookup"><span data-stu-id="21b44-143">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="21b44-144">rowHidden</span><span class="sxs-lookup"><span data-stu-id="21b44-144">rowHidden</span></span>|<span data-ttu-id="21b44-145">booliano</span><span class="sxs-lookup"><span data-stu-id="21b44-145">boolean</span></span>|<span data-ttu-id="21b44-146">Representa se todas as linhas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="21b44-146">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="21b44-147">values</span><span class="sxs-lookup"><span data-stu-id="21b44-147">values</span></span>|<span data-ttu-id="21b44-148">json</span><span class="sxs-lookup"><span data-stu-id="21b44-148">json</span></span>|<span data-ttu-id="21b44-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="21b44-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="21b44-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b44-152">Response</span></span>

<span data-ttu-id="21b44-153">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Range](../resources/range.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21b44-153">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21b44-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21b44-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21b44-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21b44-155">Request</span></span>
<span data-ttu-id="21b44-p106">Este é um exemplo da solicitação. Atualiza um intervalo: valores, formato de número e fórmula. A entrada `null` é para instruir a API a ignorar a célula para esta entrada específica. Os valores, o formato de número e as fórmulas podem ser atualizados independentemente ou combinados na mesma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="21b44-p106">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="21b44-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b44-160">Response</span></span>
<span data-ttu-id="21b44-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21b44-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

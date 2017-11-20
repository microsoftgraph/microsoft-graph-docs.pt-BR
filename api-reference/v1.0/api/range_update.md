# <a name="update-range"></a><span data-ttu-id="6ef9e-101">Intervalo de atualização</span><span class="sxs-lookup"><span data-stu-id="6ef9e-101">Update range</span></span>

<span data-ttu-id="6ef9e-102">Atualize as propriedades do objeto range.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ef9e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ef9e-103">Permissions</span></span>
<span data-ttu-id="6ef9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ef9e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ef9e-106">Permission type</span></span>      | <span data-ttu-id="6ef9e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ef9e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ef9e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ef9e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6ef9e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ef9e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ef9e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ef9e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ef9e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-111">Not supported.</span></span>    |
|<span data-ttu-id="6ef9e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ef9e-112">Application</span></span> | <span data-ttu-id="6ef9e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ef9e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ef9e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="6ef9e-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6ef9e-115">Optional request headers</span></span>
| <span data-ttu-id="6ef9e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6ef9e-116">Name</span></span>       | <span data-ttu-id="6ef9e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ef9e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6ef9e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ef9e-118">Authorization</span></span>  | <span data-ttu-id="6ef9e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ef9e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ef9e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ef9e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ef9e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ef9e-124">Request body</span></span>
<span data-ttu-id="6ef9e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6ef9e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ef9e-128">Property</span></span>     | <span data-ttu-id="6ef9e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ef9e-129">Type</span></span>   |<span data-ttu-id="6ef9e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ef9e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ef9e-131">columnHidden</span><span class="sxs-lookup"><span data-stu-id="6ef9e-131">columnHidden</span></span>|<span data-ttu-id="6ef9e-132">booliano</span><span class="sxs-lookup"><span data-stu-id="6ef9e-132">boolean</span></span>|<span data-ttu-id="6ef9e-133">Representa se todas as colunas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-133">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="6ef9e-134">fórmulas</span><span class="sxs-lookup"><span data-stu-id="6ef9e-134">formulas</span></span>|<span data-ttu-id="6ef9e-135">json</span><span class="sxs-lookup"><span data-stu-id="6ef9e-135">json</span></span>|<span data-ttu-id="6ef9e-136">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-136">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="6ef9e-137">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="6ef9e-137">formulasLocal</span></span>|<span data-ttu-id="6ef9e-138">json</span><span class="sxs-lookup"><span data-stu-id="6ef9e-138">json</span></span>|<span data-ttu-id="6ef9e-p105">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="6ef9e-141">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="6ef9e-141">formulasR1C1</span></span>|<span data-ttu-id="6ef9e-142">json</span><span class="sxs-lookup"><span data-stu-id="6ef9e-142">json</span></span>|<span data-ttu-id="6ef9e-143">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-143">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="6ef9e-144">numberFormat</span><span class="sxs-lookup"><span data-stu-id="6ef9e-144">numberFormat</span></span>|<span data-ttu-id="6ef9e-145">json</span><span class="sxs-lookup"><span data-stu-id="6ef9e-145">json</span></span>|<span data-ttu-id="6ef9e-146">Representa o código de formato de número do Excel para determinada célula.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-146">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="6ef9e-147">rowHidden</span><span class="sxs-lookup"><span data-stu-id="6ef9e-147">rowHidden</span></span>|<span data-ttu-id="6ef9e-148">booliano</span><span class="sxs-lookup"><span data-stu-id="6ef9e-148">boolean</span></span>|<span data-ttu-id="6ef9e-149">Representa se todas as linhas do intervalo atual estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-149">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="6ef9e-150">values</span><span class="sxs-lookup"><span data-stu-id="6ef9e-150">values</span></span>|<span data-ttu-id="6ef9e-151">json</span><span class="sxs-lookup"><span data-stu-id="6ef9e-151">json</span></span>|<span data-ttu-id="6ef9e-p106">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="6ef9e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ef9e-155">Response</span></span>

<span data-ttu-id="6ef9e-156">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Range](../resources/range.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-156">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ef9e-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ef9e-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ef9e-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ef9e-158">Request</span></span>
<span data-ttu-id="6ef9e-p107">Este é um exemplo da solicitação. Atualiza um intervalo: valores, formato de número e fórmula. A entrada `null` é para instruir a API a ignorar a célula para esta entrada específica. Os valores, o formato de número e as fórmulas podem ser atualizados independentemente ou combinados na mesma chamada à API.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="6ef9e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ef9e-163">Response</span></span>
<span data-ttu-id="6ef9e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ef9e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

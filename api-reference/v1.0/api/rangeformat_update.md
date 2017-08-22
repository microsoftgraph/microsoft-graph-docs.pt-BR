# <a name="update-rangeformat"></a><span data-ttu-id="71d60-101">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="71d60-101">Update rangeformat</span></span>

<span data-ttu-id="71d60-102">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="71d60-102">Update the properties of rangeformat object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71d60-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71d60-103">Prerequisites</span></span>
<span data-ttu-id="71d60-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="71d60-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="71d60-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71d60-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="71d60-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71d60-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(<address>)/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="71d60-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="71d60-107">Optional request headers</span></span>
| <span data-ttu-id="71d60-108">Nome</span><span class="sxs-lookup"><span data-stu-id="71d60-108">Name</span></span>       | <span data-ttu-id="71d60-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d60-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="71d60-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="71d60-110">Authorization</span></span>  | <span data-ttu-id="71d60-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71d60-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="71d60-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71d60-113">Request body</span></span>
<span data-ttu-id="71d60-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="71d60-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71d60-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71d60-117">Property</span></span>     | <span data-ttu-id="71d60-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="71d60-118">Type</span></span>   |<span data-ttu-id="71d60-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d60-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71d60-120">columnWidth</span><span class="sxs-lookup"><span data-stu-id="71d60-120">columnWidth</span></span>|<span data-ttu-id="71d60-121">double</span><span class="sxs-lookup"><span data-stu-id="71d60-121">double</span></span>|<span data-ttu-id="71d60-p103">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="71d60-p103">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="71d60-124">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="71d60-124">horizontalAlignment</span></span>|<span data-ttu-id="71d60-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71d60-125">string</span></span>|<span data-ttu-id="71d60-p104">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="71d60-p104">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="71d60-128">rowHeight</span><span class="sxs-lookup"><span data-stu-id="71d60-128">rowHeight</span></span>|<span data-ttu-id="71d60-129">double</span><span class="sxs-lookup"><span data-stu-id="71d60-129">double</span></span>|<span data-ttu-id="71d60-p105">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="71d60-p105">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="71d60-132">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="71d60-132">verticalAlignment</span></span>|<span data-ttu-id="71d60-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71d60-133">string</span></span>|<span data-ttu-id="71d60-p106">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="71d60-p106">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="71d60-136">wrapText</span><span class="sxs-lookup"><span data-stu-id="71d60-136">wrapText</span></span>|<span data-ttu-id="71d60-137">booliano</span><span class="sxs-lookup"><span data-stu-id="71d60-137">boolean</span></span>|<span data-ttu-id="71d60-p107">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="71d60-p107">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="71d60-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="71d60-140">Response</span></span>

<span data-ttu-id="71d60-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71d60-141">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71d60-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71d60-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71d60-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71d60-143">Request</span></span>
<span data-ttu-id="71d60-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71d60-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```
##### <a name="response"></a><span data-ttu-id="71d60-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="71d60-145">Response</span></span>
<span data-ttu-id="71d60-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71d60-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
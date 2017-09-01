# <a name="update-rangeformat"></a><span data-ttu-id="c308c-101">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="c308c-101">Update rangeformat</span></span>

<span data-ttu-id="c308c-102">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="c308c-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c308c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c308c-103">Permissions</span></span>
<span data-ttu-id="c308c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c308c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c308c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c308c-106">Permission type</span></span>      | <span data-ttu-id="c308c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c308c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c308c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c308c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c308c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c308c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c308c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c308c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c308c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c308c-111">Not supported.</span></span>    |
|<span data-ttu-id="c308c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c308c-112">Application</span></span> | <span data-ttu-id="c308c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c308c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c308c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c308c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(<address>)/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="c308c-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c308c-115">Optional request headers</span></span>
| <span data-ttu-id="c308c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="c308c-116">Name</span></span>       | <span data-ttu-id="c308c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c308c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c308c-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="c308c-118">Authorization</span></span>  | <span data-ttu-id="c308c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c308c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c308c-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c308c-121">Request body</span></span>
<span data-ttu-id="c308c-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c308c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c308c-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c308c-125">Property</span></span>     | <span data-ttu-id="c308c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c308c-126">Type</span></span>   |<span data-ttu-id="c308c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c308c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c308c-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="c308c-128">columnWidth</span></span>|<span data-ttu-id="c308c-129">double</span><span class="sxs-lookup"><span data-stu-id="c308c-129">double</span></span>|<span data-ttu-id="c308c-p104">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="c308c-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="c308c-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="c308c-132">horizontalAlignment</span></span>|<span data-ttu-id="c308c-133">string</span><span class="sxs-lookup"><span data-stu-id="c308c-133">string</span></span>|<span data-ttu-id="c308c-p105">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="c308c-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="c308c-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="c308c-136">rowHeight</span></span>|<span data-ttu-id="c308c-137">double</span><span class="sxs-lookup"><span data-stu-id="c308c-137">double</span></span>|<span data-ttu-id="c308c-p106">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="c308c-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="c308c-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="c308c-140">verticalAlignment</span></span>|<span data-ttu-id="c308c-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c308c-141">string</span></span>|<span data-ttu-id="c308c-p107">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="c308c-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="c308c-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="c308c-144">wrapText</span></span>|<span data-ttu-id="c308c-145">booliano</span><span class="sxs-lookup"><span data-stu-id="c308c-145">boolean</span></span>|<span data-ttu-id="c308c-p108">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="c308c-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="c308c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c308c-148">Response</span></span>

<span data-ttu-id="c308c-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c308c-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c308c-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c308c-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c308c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c308c-151">Request</span></span>
<span data-ttu-id="c308c-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c308c-152">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c308c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c308c-153">Response</span></span>
<span data-ttu-id="c308c-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c308c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
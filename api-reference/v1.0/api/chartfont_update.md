# <a name="update-chartfont"></a><span data-ttu-id="9a50f-101">Atualizar chartfont</span><span class="sxs-lookup"><span data-stu-id="9a50f-101">Update chartfont</span></span>

<span data-ttu-id="9a50f-102">Atualiza as propriedades do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="9a50f-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a50f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a50f-103">Permissions</span></span>
<span data-ttu-id="9a50f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a50f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a50f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a50f-106">Permission type</span></span>      | <span data-ttu-id="9a50f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a50f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a50f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a50f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9a50f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a50f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a50f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a50f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a50f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a50f-111">Not supported.</span></span>    |
|<span data-ttu-id="9a50f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a50f-112">Application</span></span> | <span data-ttu-id="9a50f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a50f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a50f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a50f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="9a50f-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="9a50f-115">Optional request headers</span></span>
| <span data-ttu-id="9a50f-116">Nome</span><span class="sxs-lookup"><span data-stu-id="9a50f-116">Name</span></span>       | <span data-ttu-id="9a50f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a50f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a50f-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a50f-118">Authorization</span></span>  | <span data-ttu-id="9a50f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a50f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a50f-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a50f-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a50f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a50f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a50f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a50f-124">Request body</span></span>
<span data-ttu-id="9a50f-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9a50f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a50f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a50f-128">Property</span></span>     | <span data-ttu-id="9a50f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a50f-129">Type</span></span>   |<span data-ttu-id="9a50f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a50f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a50f-131">bold</span><span class="sxs-lookup"><span data-stu-id="9a50f-131">bold</span></span>|<span data-ttu-id="9a50f-132">booliano</span><span class="sxs-lookup"><span data-stu-id="9a50f-132">boolean</span></span>|<span data-ttu-id="9a50f-133">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="9a50f-133">Represents the bold status of font.</span></span>|
|<span data-ttu-id="9a50f-134">color</span><span class="sxs-lookup"><span data-stu-id="9a50f-134">color</span></span>|<span data-ttu-id="9a50f-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a50f-135">string</span></span>|<span data-ttu-id="9a50f-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="9a50f-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="9a50f-139">italic</span><span class="sxs-lookup"><span data-stu-id="9a50f-139">italic</span></span>|<span data-ttu-id="9a50f-140">booliano</span><span class="sxs-lookup"><span data-stu-id="9a50f-140">boolean</span></span>|<span data-ttu-id="9a50f-141">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="9a50f-141">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="9a50f-142">name</span><span class="sxs-lookup"><span data-stu-id="9a50f-142">name</span></span>|<span data-ttu-id="9a50f-143">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a50f-143">string</span></span>|<span data-ttu-id="9a50f-144">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="9a50f-144">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="9a50f-145">size</span><span class="sxs-lookup"><span data-stu-id="9a50f-145">size</span></span>|<span data-ttu-id="9a50f-146">Double</span><span class="sxs-lookup"><span data-stu-id="9a50f-146">double</span></span>|<span data-ttu-id="9a50f-147">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="9a50f-147">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="9a50f-148">underline</span><span class="sxs-lookup"><span data-stu-id="9a50f-148">underline</span></span>|<span data-ttu-id="9a50f-149">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a50f-149">string</span></span>|<span data-ttu-id="9a50f-150">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="9a50f-150">Returns or sets the type of underline applied to the font.</span></span> <span data-ttu-id="9a50f-151">Os valores possíveis são: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="9a50f-151">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="9a50f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a50f-152">Response</span></span>

<span data-ttu-id="9a50f-153">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [WorkbookChartFont](../resources/chartfont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a50f-153">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a50f-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a50f-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a50f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a50f-155">Request</span></span>
<span data-ttu-id="9a50f-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a50f-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="9a50f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a50f-157">Response</span></span>
<span data-ttu-id="9a50f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a50f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
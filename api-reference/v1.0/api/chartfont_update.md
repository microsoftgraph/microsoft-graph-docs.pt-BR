# <a name="update-chartfont"></a><span data-ttu-id="9ca52-101">Atualizar chartfont</span><span class="sxs-lookup"><span data-stu-id="9ca52-101">Update chartfont</span></span>

<span data-ttu-id="9ca52-102">Atualiza as propriedades do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="9ca52-102">Update the properties of chartfont object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ca52-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ca52-103">Prerequisites</span></span>
<span data-ttu-id="9ca52-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="9ca52-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="9ca52-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ca52-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="9ca52-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ca52-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="9ca52-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="9ca52-107">Optional request headers</span></span>
| <span data-ttu-id="9ca52-108">Nome</span><span class="sxs-lookup"><span data-stu-id="9ca52-108">Name</span></span>       | <span data-ttu-id="9ca52-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ca52-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9ca52-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ca52-110">Authorization</span></span>  | <span data-ttu-id="9ca52-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ca52-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9ca52-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca52-113">Request body</span></span>
<span data-ttu-id="9ca52-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9ca52-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ca52-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ca52-117">Property</span></span>     | <span data-ttu-id="9ca52-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ca52-118">Type</span></span>   |<span data-ttu-id="9ca52-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ca52-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ca52-120">bold</span><span class="sxs-lookup"><span data-stu-id="9ca52-120">bold</span></span>|<span data-ttu-id="9ca52-121">booliano</span><span class="sxs-lookup"><span data-stu-id="9ca52-121">boolean</span></span>|<span data-ttu-id="9ca52-122">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="9ca52-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="9ca52-123">color</span><span class="sxs-lookup"><span data-stu-id="9ca52-123">color</span></span>|<span data-ttu-id="9ca52-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ca52-124">string</span></span>|<span data-ttu-id="9ca52-p103">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="9ca52-p103">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="9ca52-128">italic</span><span class="sxs-lookup"><span data-stu-id="9ca52-128">italic</span></span>|<span data-ttu-id="9ca52-129">booliano</span><span class="sxs-lookup"><span data-stu-id="9ca52-129">boolean</span></span>|<span data-ttu-id="9ca52-130">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="9ca52-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="9ca52-131">name</span><span class="sxs-lookup"><span data-stu-id="9ca52-131">name</span></span>|<span data-ttu-id="9ca52-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ca52-132">string</span></span>|<span data-ttu-id="9ca52-133">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="9ca52-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="9ca52-134">size</span><span class="sxs-lookup"><span data-stu-id="9ca52-134">size</span></span>|<span data-ttu-id="9ca52-135">Double</span><span class="sxs-lookup"><span data-stu-id="9ca52-135">double</span></span>|<span data-ttu-id="9ca52-136">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="9ca52-136">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="9ca52-137">underline</span><span class="sxs-lookup"><span data-stu-id="9ca52-137">underline</span></span>|<span data-ttu-id="9ca52-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ca52-138">string</span></span>|<span data-ttu-id="9ca52-p104">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="9ca52-p104">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="9ca52-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ca52-141">Response</span></span>

<span data-ttu-id="9ca52-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartFont](../resources/chartfont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ca52-142">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ca52-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ca52-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ca52-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca52-144">Request</span></span>
<span data-ttu-id="9ca52-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ca52-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
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
##### <a name="response"></a><span data-ttu-id="9ca52-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ca52-146">Response</span></span>
<span data-ttu-id="9ca52-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ca52-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
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
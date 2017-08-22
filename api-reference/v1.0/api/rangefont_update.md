# <a name="update-rangefont"></a><span data-ttu-id="91a94-101">Atualizar rangefont</span><span class="sxs-lookup"><span data-stu-id="91a94-101">Update rangefont</span></span>

<span data-ttu-id="91a94-102">Atualize as propriedades do objeto rangefont.</span><span class="sxs-lookup"><span data-stu-id="91a94-102">Update the properties of rangefont object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91a94-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91a94-103">Prerequisites</span></span>
<span data-ttu-id="91a94-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="91a94-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="91a94-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91a94-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="91a94-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91a94-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="91a94-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="91a94-107">Optional request headers</span></span>
| <span data-ttu-id="91a94-108">Nome</span><span class="sxs-lookup"><span data-stu-id="91a94-108">Name</span></span>       | <span data-ttu-id="91a94-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="91a94-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="91a94-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="91a94-110">Authorization</span></span>  | <span data-ttu-id="91a94-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91a94-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="91a94-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91a94-113">Request body</span></span>
<span data-ttu-id="91a94-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="91a94-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91a94-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91a94-117">Property</span></span>     | <span data-ttu-id="91a94-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="91a94-118">Type</span></span>   |<span data-ttu-id="91a94-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="91a94-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91a94-120">bold</span><span class="sxs-lookup"><span data-stu-id="91a94-120">bold</span></span>|<span data-ttu-id="91a94-121">booliano</span><span class="sxs-lookup"><span data-stu-id="91a94-121">boolean</span></span>|<span data-ttu-id="91a94-122">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="91a94-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="91a94-123">color</span><span class="sxs-lookup"><span data-stu-id="91a94-123">color</span></span>|<span data-ttu-id="91a94-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91a94-124">string</span></span>|<span data-ttu-id="91a94-p103">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="91a94-p103">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="91a94-128">italic</span><span class="sxs-lookup"><span data-stu-id="91a94-128">italic</span></span>|<span data-ttu-id="91a94-129">booliano</span><span class="sxs-lookup"><span data-stu-id="91a94-129">boolean</span></span>|<span data-ttu-id="91a94-130">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="91a94-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="91a94-131">name</span><span class="sxs-lookup"><span data-stu-id="91a94-131">name</span></span>|<span data-ttu-id="91a94-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91a94-132">string</span></span>|<span data-ttu-id="91a94-133">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="91a94-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="91a94-134">size</span><span class="sxs-lookup"><span data-stu-id="91a94-134">size</span></span>|<span data-ttu-id="91a94-135">Double</span><span class="sxs-lookup"><span data-stu-id="91a94-135">double</span></span>|<span data-ttu-id="91a94-136">Font Size</span><span class="sxs-lookup"><span data-stu-id="91a94-136">Font size.</span></span>|
|<span data-ttu-id="91a94-137">underline</span><span class="sxs-lookup"><span data-stu-id="91a94-137">underline</span></span>|<span data-ttu-id="91a94-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91a94-138">string</span></span>|<span data-ttu-id="91a94-p104">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="91a94-p104">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="91a94-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="91a94-141">Response</span></span>

<span data-ttu-id="91a94-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFont](../resources/rangefont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91a94-142">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91a94-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91a94-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91a94-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91a94-144">Request</span></span>
<span data-ttu-id="91a94-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91a94-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="91a94-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="91a94-146">Response</span></span>
<span data-ttu-id="91a94-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91a94-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
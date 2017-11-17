# <a name="update-chartfont"></a><span data-ttu-id="b87f8-101">Atualizar chartfont</span><span class="sxs-lookup"><span data-stu-id="b87f8-101">Update chartfont</span></span>

<span data-ttu-id="b87f8-102">Atualiza as propriedades do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="b87f8-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b87f8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b87f8-103">Permissions</span></span>
<span data-ttu-id="b87f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b87f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b87f8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b87f8-106">Permission type</span></span>      | <span data-ttu-id="b87f8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b87f8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b87f8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b87f8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b87f8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b87f8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b87f8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b87f8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b87f8-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b87f8-111">Not supported.</span></span>    |
|<span data-ttu-id="b87f8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b87f8-112">Application</span></span> | <span data-ttu-id="b87f8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b87f8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b87f8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b87f8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="b87f8-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b87f8-115">Optional request headers</span></span>
| <span data-ttu-id="b87f8-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b87f8-116">Name</span></span>       | <span data-ttu-id="b87f8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b87f8-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b87f8-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="b87f8-118">Authorization</span></span>  | <span data-ttu-id="b87f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b87f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b87f8-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b87f8-121">Request body</span></span>
<span data-ttu-id="b87f8-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b87f8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b87f8-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b87f8-125">Property</span></span>     | <span data-ttu-id="b87f8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b87f8-126">Type</span></span>   |<span data-ttu-id="b87f8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b87f8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b87f8-128">bold</span><span class="sxs-lookup"><span data-stu-id="b87f8-128">bold</span></span>|<span data-ttu-id="b87f8-129">booliano</span><span class="sxs-lookup"><span data-stu-id="b87f8-129">boolean</span></span>|<span data-ttu-id="b87f8-130">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="b87f8-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="b87f8-131">color</span><span class="sxs-lookup"><span data-stu-id="b87f8-131">color</span></span>|<span data-ttu-id="b87f8-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b87f8-132">string</span></span>|<span data-ttu-id="b87f8-p104">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="b87f8-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="b87f8-136">italic</span><span class="sxs-lookup"><span data-stu-id="b87f8-136">italic</span></span>|<span data-ttu-id="b87f8-137">booliano</span><span class="sxs-lookup"><span data-stu-id="b87f8-137">boolean</span></span>|<span data-ttu-id="b87f8-138">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="b87f8-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="b87f8-139">name</span><span class="sxs-lookup"><span data-stu-id="b87f8-139">name</span></span>|<span data-ttu-id="b87f8-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b87f8-140">string</span></span>|<span data-ttu-id="b87f8-141">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="b87f8-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="b87f8-142">size</span><span class="sxs-lookup"><span data-stu-id="b87f8-142">size</span></span>|<span data-ttu-id="b87f8-143">Double</span><span class="sxs-lookup"><span data-stu-id="b87f8-143">double</span></span>|<span data-ttu-id="b87f8-144">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="b87f8-144">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="b87f8-145">underline</span><span class="sxs-lookup"><span data-stu-id="b87f8-145">underline</span></span>|<span data-ttu-id="b87f8-146">string</span><span class="sxs-lookup"><span data-stu-id="b87f8-146">string</span></span>|<span data-ttu-id="b87f8-p105">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="b87f8-p105">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="b87f8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b87f8-149">Response</span></span>

<span data-ttu-id="b87f8-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartFont](../resources/chartfont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b87f8-150">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b87f8-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b87f8-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b87f8-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b87f8-152">Request</span></span>
<span data-ttu-id="b87f8-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b87f8-153">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b87f8-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b87f8-154">Response</span></span>
<span data-ttu-id="b87f8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b87f8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
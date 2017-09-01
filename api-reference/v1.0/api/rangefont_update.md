# <a name="update-rangefont"></a><span data-ttu-id="5ad6e-101">Atualizar rangefont</span><span class="sxs-lookup"><span data-stu-id="5ad6e-101">Update rangefont</span></span>

<span data-ttu-id="5ad6e-102">Atualize as propriedades do objeto rangefont.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-102">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ad6e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ad6e-103">Permissions</span></span>
<span data-ttu-id="5ad6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ad6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ad6e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ad6e-106">Permission type</span></span>      | <span data-ttu-id="5ad6e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ad6e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ad6e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ad6e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5ad6e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ad6e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ad6e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ad6e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ad6e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-111">Not supported.</span></span>    |
|<span data-ttu-id="5ad6e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ad6e-112">Application</span></span> | <span data-ttu-id="5ad6e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ad6e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ad6e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="5ad6e-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5ad6e-115">Optional request headers</span></span>
| <span data-ttu-id="5ad6e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5ad6e-116">Name</span></span>       | <span data-ttu-id="5ad6e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ad6e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5ad6e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ad6e-118">Authorization</span></span>  | <span data-ttu-id="5ad6e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ad6e-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ad6e-121">Request body</span></span>
<span data-ttu-id="5ad6e-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ad6e-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ad6e-125">Property</span></span>     | <span data-ttu-id="5ad6e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ad6e-126">Type</span></span>   |<span data-ttu-id="5ad6e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ad6e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ad6e-128">bold</span><span class="sxs-lookup"><span data-stu-id="5ad6e-128">bold</span></span>|<span data-ttu-id="5ad6e-129">booliano</span><span class="sxs-lookup"><span data-stu-id="5ad6e-129">boolean</span></span>|<span data-ttu-id="5ad6e-130">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="5ad6e-131">color</span><span class="sxs-lookup"><span data-stu-id="5ad6e-131">color</span></span>|<span data-ttu-id="5ad6e-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ad6e-132">string</span></span>|<span data-ttu-id="5ad6e-p104">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="5ad6e-136">italic</span><span class="sxs-lookup"><span data-stu-id="5ad6e-136">italic</span></span>|<span data-ttu-id="5ad6e-137">booliano</span><span class="sxs-lookup"><span data-stu-id="5ad6e-137">boolean</span></span>|<span data-ttu-id="5ad6e-138">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="5ad6e-139">name</span><span class="sxs-lookup"><span data-stu-id="5ad6e-139">name</span></span>|<span data-ttu-id="5ad6e-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ad6e-140">string</span></span>|<span data-ttu-id="5ad6e-141">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="5ad6e-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="5ad6e-142">size</span><span class="sxs-lookup"><span data-stu-id="5ad6e-142">size</span></span>|<span data-ttu-id="5ad6e-143">Double</span><span class="sxs-lookup"><span data-stu-id="5ad6e-143">double</span></span>|<span data-ttu-id="5ad6e-144">Font Size</span><span class="sxs-lookup"><span data-stu-id="5ad6e-144">Font size.</span></span>|
|<span data-ttu-id="5ad6e-145">underline</span><span class="sxs-lookup"><span data-stu-id="5ad6e-145">underline</span></span>|<span data-ttu-id="5ad6e-146">string</span><span class="sxs-lookup"><span data-stu-id="5ad6e-146">string</span></span>|<span data-ttu-id="5ad6e-p105">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-p105">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="5ad6e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ad6e-149">Response</span></span>

<span data-ttu-id="5ad6e-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFont](../resources/rangefont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-150">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ad6e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ad6e-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ad6e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ad6e-152">Request</span></span>
<span data-ttu-id="5ad6e-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-153">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5ad6e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ad6e-154">Response</span></span>
<span data-ttu-id="5ad6e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ad6e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
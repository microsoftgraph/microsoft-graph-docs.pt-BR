# <a name="update-rangeborder"></a><span data-ttu-id="0498f-101">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="0498f-101">Update rangeborder</span></span>

<span data-ttu-id="0498f-102">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="0498f-102">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0498f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="0498f-103">Permissions</span></span>
<span data-ttu-id="0498f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0498f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0498f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0498f-106">Permission type</span></span>      | <span data-ttu-id="0498f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0498f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0498f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0498f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0498f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0498f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0498f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0498f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0498f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0498f-111">Not supported.</span></span>    |
|<span data-ttu-id="0498f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0498f-112">Application</span></span> | <span data-ttu-id="0498f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0498f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0498f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0498f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0498f-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0498f-115">Optional request headers</span></span>
| <span data-ttu-id="0498f-116">Nome</span><span class="sxs-lookup"><span data-stu-id="0498f-116">Name</span></span>       | <span data-ttu-id="0498f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0498f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0498f-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="0498f-118">Authorization</span></span>  | <span data-ttu-id="0498f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0498f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0498f-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0498f-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="0498f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0498f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0498f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0498f-124">Request body</span></span>
<span data-ttu-id="0498f-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0498f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0498f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0498f-128">Property</span></span>     | <span data-ttu-id="0498f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0498f-129">Type</span></span>   |<span data-ttu-id="0498f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0498f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0498f-131">color</span><span class="sxs-lookup"><span data-stu-id="0498f-131">color</span></span>|<span data-ttu-id="0498f-132">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="0498f-132">string</span></span>|<span data-ttu-id="0498f-133">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="0498f-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="0498f-134">style</span><span class="sxs-lookup"><span data-stu-id="0498f-134">style</span></span>|<span data-ttu-id="0498f-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="0498f-135">string</span></span>|<span data-ttu-id="0498f-136">Uma das constantes do estilo da linha, especificando o estilo da linha da borda.</span><span class="sxs-lookup"><span data-stu-id="0498f-136">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="0498f-137">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="0498f-137">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="0498f-138">weight</span><span class="sxs-lookup"><span data-stu-id="0498f-138">weight</span></span>|<span data-ttu-id="0498f-139">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="0498f-139">string</span></span>|<span data-ttu-id="0498f-140">Especifica o peso da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="0498f-140">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="0498f-141">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="0498f-141">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="0498f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0498f-142">Response</span></span>

<span data-ttu-id="0498f-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0498f-143">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0498f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0498f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0498f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0498f-145">Request</span></span>
<span data-ttu-id="0498f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0498f-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="0498f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0498f-147">Response</span></span>
<span data-ttu-id="0498f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0498f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
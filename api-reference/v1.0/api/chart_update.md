# <a name="update-chart"></a><span data-ttu-id="3fc44-101">Atualizar gráfico</span><span class="sxs-lookup"><span data-stu-id="3fc44-101">Update chart</span></span>

<span data-ttu-id="3fc44-102">Atualiza as propriedades do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="3fc44-102">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3fc44-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fc44-103">Permissions</span></span>
<span data-ttu-id="3fc44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fc44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3fc44-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fc44-106">Permission type</span></span>      | <span data-ttu-id="3fc44-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fc44-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fc44-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fc44-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3fc44-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fc44-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3fc44-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fc44-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fc44-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fc44-111">Not supported.</span></span>    |
|<span data-ttu-id="3fc44-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fc44-112">Application</span></span> | <span data-ttu-id="3fc44-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fc44-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fc44-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fc44-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="3fc44-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3fc44-115">Optional request headers</span></span>
| <span data-ttu-id="3fc44-116">Nome</span><span class="sxs-lookup"><span data-stu-id="3fc44-116">Name</span></span>       | <span data-ttu-id="3fc44-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fc44-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3fc44-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fc44-118">Authorization</span></span>  | <span data-ttu-id="3fc44-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fc44-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fc44-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3fc44-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3fc44-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3fc44-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fc44-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc44-124">Request body</span></span>
<span data-ttu-id="3fc44-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3fc44-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3fc44-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fc44-128">Property</span></span>     | <span data-ttu-id="3fc44-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fc44-129">Type</span></span>   |<span data-ttu-id="3fc44-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fc44-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fc44-131">height</span><span class="sxs-lookup"><span data-stu-id="3fc44-131">height</span></span>|<span data-ttu-id="3fc44-132">Double</span><span class="sxs-lookup"><span data-stu-id="3fc44-132">double</span></span>|<span data-ttu-id="3fc44-133">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="3fc44-133">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="3fc44-134">left</span><span class="sxs-lookup"><span data-stu-id="3fc44-134">left</span></span>|<span data-ttu-id="3fc44-135">Double</span><span class="sxs-lookup"><span data-stu-id="3fc44-135">double</span></span>|<span data-ttu-id="3fc44-136">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="3fc44-136">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="3fc44-137">name</span><span class="sxs-lookup"><span data-stu-id="3fc44-137">name</span></span>|<span data-ttu-id="3fc44-138">string</span><span class="sxs-lookup"><span data-stu-id="3fc44-138">string</span></span>|<span data-ttu-id="3fc44-139">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="3fc44-139">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="3fc44-140">top</span><span class="sxs-lookup"><span data-stu-id="3fc44-140">top</span></span>|<span data-ttu-id="3fc44-141">Double</span><span class="sxs-lookup"><span data-stu-id="3fc44-141">double</span></span>|<span data-ttu-id="3fc44-142">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="3fc44-142">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="3fc44-143">width</span><span class="sxs-lookup"><span data-stu-id="3fc44-143">width</span></span>|<span data-ttu-id="3fc44-144">Double</span><span class="sxs-lookup"><span data-stu-id="3fc44-144">double</span></span>|<span data-ttu-id="3fc44-145">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="3fc44-145">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="3fc44-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fc44-146">Response</span></span>

<span data-ttu-id="3fc44-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Chart](../resources/chart.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fc44-147">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fc44-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fc44-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fc44-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc44-149">Request</span></span>
<span data-ttu-id="3fc44-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fc44-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="3fc44-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fc44-151">Response</span></span>
<span data-ttu-id="3fc44-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fc44-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="update-chartlegend"></a><span data-ttu-id="2faab-101">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="2faab-101">Update chartlegend</span></span>

<span data-ttu-id="2faab-102">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="2faab-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2faab-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2faab-103">Permissions</span></span>
<span data-ttu-id="2faab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2faab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2faab-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2faab-106">Permission type</span></span>      | <span data-ttu-id="2faab-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2faab-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2faab-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2faab-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2faab-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2faab-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2faab-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2faab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2faab-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2faab-111">Not supported.</span></span>    |
|<span data-ttu-id="2faab-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2faab-112">Application</span></span> | <span data-ttu-id="2faab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2faab-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2faab-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2faab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="2faab-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2faab-115">Optional request headers</span></span>
| <span data-ttu-id="2faab-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2faab-116">Name</span></span>       | <span data-ttu-id="2faab-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2faab-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2faab-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2faab-118">Authorization</span></span>  | <span data-ttu-id="2faab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2faab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2faab-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2faab-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2faab-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2faab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2faab-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2faab-124">Request body</span></span>
<span data-ttu-id="2faab-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2faab-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2faab-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2faab-128">Property</span></span>     | <span data-ttu-id="2faab-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2faab-129">Type</span></span>   |<span data-ttu-id="2faab-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2faab-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2faab-131">overlay</span><span class="sxs-lookup"><span data-stu-id="2faab-131">overlay</span></span>|<span data-ttu-id="2faab-132">booliano</span><span class="sxs-lookup"><span data-stu-id="2faab-132">boolean</span></span>|<span data-ttu-id="2faab-133">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2faab-133">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="2faab-134">posição</span><span class="sxs-lookup"><span data-stu-id="2faab-134">position</span></span>|<span data-ttu-id="2faab-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="2faab-135">string</span></span>|<span data-ttu-id="2faab-136">Representa a posição da legenda no gráfico.</span><span class="sxs-lookup"><span data-stu-id="2faab-136">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="2faab-137">Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="2faab-137">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="2faab-138">visible</span><span class="sxs-lookup"><span data-stu-id="2faab-138">visible</span></span>|<span data-ttu-id="2faab-139">booliano</span><span class="sxs-lookup"><span data-stu-id="2faab-139">boolean</span></span>|<span data-ttu-id="2faab-140">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="2faab-140">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="2faab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2faab-141">Response</span></span>

<span data-ttu-id="2faab-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto atualizado [WorkbookChartLegend](../resources/chartlegend.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2faab-142">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2faab-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2faab-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2faab-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2faab-144">Request</span></span>
<span data-ttu-id="2faab-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2faab-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="2faab-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2faab-146">Response</span></span>
<span data-ttu-id="2faab-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2faab-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
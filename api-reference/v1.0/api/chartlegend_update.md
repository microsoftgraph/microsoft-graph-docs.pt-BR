# <a name="update-chartlegend"></a><span data-ttu-id="6055d-101">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="6055d-101">Update chartlegend</span></span>

<span data-ttu-id="6055d-102">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="6055d-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6055d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6055d-103">Permissions</span></span>
<span data-ttu-id="6055d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6055d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6055d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6055d-106">Permission type</span></span>      | <span data-ttu-id="6055d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6055d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6055d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6055d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6055d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6055d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6055d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6055d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6055d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6055d-111">Not supported.</span></span>    |
|<span data-ttu-id="6055d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6055d-112">Application</span></span> | <span data-ttu-id="6055d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6055d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6055d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6055d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="6055d-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6055d-115">Optional request headers</span></span>
| <span data-ttu-id="6055d-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6055d-116">Name</span></span>       | <span data-ttu-id="6055d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6055d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6055d-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="6055d-118">Authorization</span></span>  | <span data-ttu-id="6055d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6055d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6055d-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6055d-121">Request body</span></span>
<span data-ttu-id="6055d-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6055d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6055d-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6055d-125">Property</span></span>     | <span data-ttu-id="6055d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6055d-126">Type</span></span>   |<span data-ttu-id="6055d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6055d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6055d-128">overlay</span><span class="sxs-lookup"><span data-stu-id="6055d-128">overlay</span></span>|<span data-ttu-id="6055d-129">booliano</span><span class="sxs-lookup"><span data-stu-id="6055d-129">boolean</span></span>|<span data-ttu-id="6055d-130">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="6055d-130">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="6055d-131">position</span><span class="sxs-lookup"><span data-stu-id="6055d-131">position</span></span>|<span data-ttu-id="6055d-132">string</span><span class="sxs-lookup"><span data-stu-id="6055d-132">string</span></span>|<span data-ttu-id="6055d-p104">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="6055d-p104">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="6055d-135">visible</span><span class="sxs-lookup"><span data-stu-id="6055d-135">visible</span></span>|<span data-ttu-id="6055d-136">booliano</span><span class="sxs-lookup"><span data-stu-id="6055d-136">boolean</span></span>|<span data-ttu-id="6055d-137">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="6055d-137">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="6055d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6055d-138">Response</span></span>

<span data-ttu-id="6055d-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartLegend](../resources/chartlegend.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6055d-139">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6055d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6055d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6055d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6055d-141">Request</span></span>
<span data-ttu-id="6055d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6055d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="6055d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6055d-143">Response</span></span>
<span data-ttu-id="6055d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6055d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
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
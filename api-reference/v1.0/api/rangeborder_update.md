# <a name="update-rangeborder"></a><span data-ttu-id="eee10-101">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="eee10-101">Update rangeborder</span></span>

<span data-ttu-id="eee10-102">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="eee10-102">Update the properties of rangeborder object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eee10-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eee10-103">Prerequisites</span></span>
<span data-ttu-id="eee10-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="eee10-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="eee10-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eee10-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="eee10-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eee10-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="eee10-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="eee10-107">Optional request headers</span></span>
| <span data-ttu-id="eee10-108">Nome</span><span class="sxs-lookup"><span data-stu-id="eee10-108">Name</span></span>       | <span data-ttu-id="eee10-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee10-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eee10-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="eee10-110">Authorization</span></span>  | <span data-ttu-id="eee10-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eee10-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="eee10-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eee10-113">Request body</span></span>
<span data-ttu-id="eee10-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eee10-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eee10-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eee10-117">Property</span></span>     | <span data-ttu-id="eee10-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="eee10-118">Type</span></span>   |<span data-ttu-id="eee10-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee10-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eee10-120">color</span><span class="sxs-lookup"><span data-stu-id="eee10-120">color</span></span>|<span data-ttu-id="eee10-121">string</span><span class="sxs-lookup"><span data-stu-id="eee10-121">string</span></span>|<span data-ttu-id="eee10-122">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="eee10-122">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="eee10-123">estilo</span><span class="sxs-lookup"><span data-stu-id="eee10-123">style</span></span>|<span data-ttu-id="eee10-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee10-124">string</span></span>|<span data-ttu-id="eee10-p103">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="eee10-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="eee10-127">weight</span><span class="sxs-lookup"><span data-stu-id="eee10-127">weight</span></span>|<span data-ttu-id="eee10-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee10-128">string</span></span>|<span data-ttu-id="eee10-p104">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="eee10-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="eee10-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee10-131">Response</span></span>

<span data-ttu-id="eee10-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eee10-132">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eee10-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eee10-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eee10-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eee10-134">Request</span></span>
<span data-ttu-id="eee10-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eee10-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="eee10-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee10-136">Response</span></span>
<span data-ttu-id="eee10-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eee10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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
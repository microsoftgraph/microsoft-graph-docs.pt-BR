# <a name="update-charttitle"></a><span data-ttu-id="88bc1-101">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="88bc1-101">Update charttitle</span></span>

<span data-ttu-id="88bc1-102">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="88bc1-102">Update the properties of charttitle object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88bc1-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88bc1-103">Prerequisites</span></span>
<span data-ttu-id="88bc1-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="88bc1-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="88bc1-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88bc1-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="88bc1-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88bc1-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="88bc1-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="88bc1-107">Optional request headers</span></span>
| <span data-ttu-id="88bc1-108">Nome</span><span class="sxs-lookup"><span data-stu-id="88bc1-108">Name</span></span>       | <span data-ttu-id="88bc1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="88bc1-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="88bc1-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="88bc1-110">Authorization</span></span>  | <span data-ttu-id="88bc1-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88bc1-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="88bc1-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88bc1-113">Request body</span></span>
<span data-ttu-id="88bc1-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="88bc1-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="88bc1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88bc1-117">Property</span></span>     | <span data-ttu-id="88bc1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="88bc1-118">Type</span></span>   |<span data-ttu-id="88bc1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="88bc1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88bc1-120">overlay</span><span class="sxs-lookup"><span data-stu-id="88bc1-120">overlay</span></span>|<span data-ttu-id="88bc1-121">booliano</span><span class="sxs-lookup"><span data-stu-id="88bc1-121">boolean</span></span>|<span data-ttu-id="88bc1-122">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="88bc1-122">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="88bc1-123">texto</span><span class="sxs-lookup"><span data-stu-id="88bc1-123">text</span></span>|<span data-ttu-id="88bc1-124">string</span><span class="sxs-lookup"><span data-stu-id="88bc1-124">string</span></span>|<span data-ttu-id="88bc1-125">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="88bc1-125">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="88bc1-126">visible</span><span class="sxs-lookup"><span data-stu-id="88bc1-126">visible</span></span>|<span data-ttu-id="88bc1-127">booliano</span><span class="sxs-lookup"><span data-stu-id="88bc1-127">boolean</span></span>|<span data-ttu-id="88bc1-128">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="88bc1-128">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="88bc1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="88bc1-129">Response</span></span>

<span data-ttu-id="88bc1-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartTitle](../resources/charttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88bc1-130">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88bc1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88bc1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88bc1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88bc1-132">Request</span></span>
<span data-ttu-id="88bc1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88bc1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="88bc1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="88bc1-134">Response</span></span>
<span data-ttu-id="88bc1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88bc1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="update-chartaxistitle"></a><span data-ttu-id="2108a-101">Atualizar chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="2108a-101">Update chartaxistitle</span></span>

<span data-ttu-id="2108a-102">Atualiza as propriedades do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="2108a-102">Update the properties of chartaxistitle object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2108a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2108a-103">Prerequisites</span></span>
<span data-ttu-id="2108a-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="2108a-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="2108a-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2108a-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="2108a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2108a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="2108a-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2108a-107">Optional request headers</span></span>
| <span data-ttu-id="2108a-108">Nome</span><span class="sxs-lookup"><span data-stu-id="2108a-108">Name</span></span>       | <span data-ttu-id="2108a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2108a-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2108a-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="2108a-110">Authorization</span></span>  | <span data-ttu-id="2108a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2108a-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2108a-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2108a-113">Request body</span></span>
<span data-ttu-id="2108a-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2108a-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2108a-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2108a-117">Property</span></span>     | <span data-ttu-id="2108a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2108a-118">Type</span></span>   |<span data-ttu-id="2108a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2108a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2108a-120">texto</span><span class="sxs-lookup"><span data-stu-id="2108a-120">text</span></span>|<span data-ttu-id="2108a-121">string</span><span class="sxs-lookup"><span data-stu-id="2108a-121">string</span></span>|<span data-ttu-id="2108a-122">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="2108a-122">Represents the axis title.</span></span>|
|<span data-ttu-id="2108a-123">visible</span><span class="sxs-lookup"><span data-stu-id="2108a-123">visible</span></span>|<span data-ttu-id="2108a-124">booliano</span><span class="sxs-lookup"><span data-stu-id="2108a-124">boolean</span></span>|<span data-ttu-id="2108a-125">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="2108a-125">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="2108a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2108a-126">Response</span></span>

<span data-ttu-id="2108a-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxisTitle](../resources/chartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2108a-127">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2108a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2108a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2108a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2108a-129">Request</span></span>
<span data-ttu-id="2108a-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2108a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="2108a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2108a-131">Response</span></span>
<span data-ttu-id="2108a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2108a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
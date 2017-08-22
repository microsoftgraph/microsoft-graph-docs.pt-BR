# <a name="update-worksheet"></a><span data-ttu-id="c0117-101">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="c0117-101">Update worksheet</span></span>

<span data-ttu-id="c0117-102">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="c0117-102">Update the properties of worksheet object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0117-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0117-103">Prerequisites</span></span>
<span data-ttu-id="c0117-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="c0117-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="c0117-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0117-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="c0117-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0117-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c0117-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c0117-107">Optional request headers</span></span>
| <span data-ttu-id="c0117-108">Nome</span><span class="sxs-lookup"><span data-stu-id="c0117-108">Name</span></span>       | <span data-ttu-id="c0117-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0117-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0117-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0117-110">Authorization</span></span>  | <span data-ttu-id="c0117-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0117-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c0117-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0117-113">Request body</span></span>
<span data-ttu-id="c0117-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0117-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0117-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0117-117">Property</span></span>     | <span data-ttu-id="c0117-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0117-118">Type</span></span>   |<span data-ttu-id="c0117-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0117-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0117-120">name</span><span class="sxs-lookup"><span data-stu-id="c0117-120">name</span></span>|<span data-ttu-id="c0117-121">string</span><span class="sxs-lookup"><span data-stu-id="c0117-121">string</span></span>|<span data-ttu-id="c0117-122">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="c0117-122">The display name of the worksheet.</span></span>|
|<span data-ttu-id="c0117-123">position</span><span class="sxs-lookup"><span data-stu-id="c0117-123">position</span></span>|<span data-ttu-id="c0117-124">int</span><span class="sxs-lookup"><span data-stu-id="c0117-124">int</span></span>|<span data-ttu-id="c0117-125">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0117-125">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="c0117-126">visibilidade</span><span class="sxs-lookup"><span data-stu-id="c0117-126">visibility</span></span>|<span data-ttu-id="c0117-127">string</span><span class="sxs-lookup"><span data-stu-id="c0117-127">string</span></span>|<span data-ttu-id="c0117-p103">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="c0117-p103">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="c0117-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0117-130">Response</span></span>

<span data-ttu-id="c0117-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0117-131">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0117-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0117-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0117-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0117-133">Request</span></span>
<span data-ttu-id="c0117-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0117-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="c0117-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0117-135">Response</span></span>
<span data-ttu-id="c0117-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0117-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
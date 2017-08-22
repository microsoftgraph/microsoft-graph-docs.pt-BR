# <a name="chart-setposition"></a><span data-ttu-id="5c6ce-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="5c6ce-101">Chart: setPosition</span></span>

<span data-ttu-id="5c6ce-102">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c6ce-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c6ce-103">Prerequisites</span></span>
<span data-ttu-id="5c6ce-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="5c6ce-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="5c6ce-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c6ce-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="5c6ce-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c6ce-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="5c6ce-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c6ce-107">Request headers</span></span>
| <span data-ttu-id="5c6ce-108">Nome</span><span class="sxs-lookup"><span data-stu-id="5c6ce-108">Name</span></span>       | <span data-ttu-id="5c6ce-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c6ce-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c6ce-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c6ce-110">Authorization</span></span>  | <span data-ttu-id="5c6ce-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5c6ce-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c6ce-113">Request body</span></span>
<span data-ttu-id="5c6ce-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c6ce-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c6ce-115">Parameter</span></span>    | <span data-ttu-id="5c6ce-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c6ce-116">Type</span></span>   |<span data-ttu-id="5c6ce-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c6ce-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c6ce-118">startCell</span><span class="sxs-lookup"><span data-stu-id="5c6ce-118">startCell</span></span>|<span data-ttu-id="5c6ce-119">string</span><span class="sxs-lookup"><span data-stu-id="5c6ce-119">string</span></span>|<span data-ttu-id="5c6ce-p102">A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-p102">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="5c6ce-123">endCell</span><span class="sxs-lookup"><span data-stu-id="5c6ce-123">endCell</span></span>|<span data-ttu-id="5c6ce-124">string</span><span class="sxs-lookup"><span data-stu-id="5c6ce-124">string</span></span>|<span data-ttu-id="5c6ce-p103">Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-p103">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="5c6ce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c6ce-128">Response</span></span>

<span data-ttu-id="5c6ce-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c6ce-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c6ce-131">Example</span></span>
<span data-ttu-id="5c6ce-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c6ce-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c6ce-133">Request</span></span>
<span data-ttu-id="5c6ce-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="5c6ce-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c6ce-135">Response</span></span>
<span data-ttu-id="5c6ce-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c6ce-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
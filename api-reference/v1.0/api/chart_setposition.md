# <a name="chart-setposition"></a><span data-ttu-id="94e3e-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="94e3e-101">Chart: setPosition</span></span>

<span data-ttu-id="94e3e-102">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="94e3e-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="94e3e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="94e3e-103">Permissions</span></span>
<span data-ttu-id="94e3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="94e3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94e3e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94e3e-106">Permission type</span></span>      | <span data-ttu-id="94e3e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94e3e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94e3e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94e3e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="94e3e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94e3e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94e3e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94e3e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94e3e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94e3e-111">Not supported.</span></span>    |
|<span data-ttu-id="94e3e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94e3e-112">Application</span></span> | <span data-ttu-id="94e3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94e3e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94e3e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94e3e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="94e3e-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94e3e-115">Request headers</span></span>
| <span data-ttu-id="94e3e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="94e3e-116">Name</span></span>       | <span data-ttu-id="94e3e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="94e3e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94e3e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="94e3e-118">Authorization</span></span>  | <span data-ttu-id="94e3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94e3e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94e3e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="94e3e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e3e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94e3e-124">Request body</span></span>
<span data-ttu-id="94e3e-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94e3e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94e3e-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94e3e-126">Parameter</span></span>    | <span data-ttu-id="94e3e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="94e3e-127">Type</span></span>   |<span data-ttu-id="94e3e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="94e3e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94e3e-129">startCell</span><span class="sxs-lookup"><span data-stu-id="94e3e-129">startCell</span></span>|<span data-ttu-id="94e3e-130">string</span><span class="sxs-lookup"><span data-stu-id="94e3e-130">string</span></span>|<span data-ttu-id="94e3e-p104">A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="94e3e-134">endCell</span><span class="sxs-lookup"><span data-stu-id="94e3e-134">endCell</span></span>|<span data-ttu-id="94e3e-135">string</span><span class="sxs-lookup"><span data-stu-id="94e3e-135">string</span></span>|<span data-ttu-id="94e3e-p105">Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="94e3e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="94e3e-139">Response</span></span>

<span data-ttu-id="94e3e-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e3e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94e3e-142">Example</span></span>
<span data-ttu-id="94e3e-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="94e3e-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94e3e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94e3e-144">Request</span></span>
<span data-ttu-id="94e3e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94e3e-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="94e3e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="94e3e-146">Response</span></span>
<span data-ttu-id="94e3e-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94e3e-147">Here is an example of the response.</span></span> 
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
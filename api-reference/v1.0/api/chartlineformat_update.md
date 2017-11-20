# <a name="update-chartlineformat"></a><span data-ttu-id="2943a-101">Atualizar chartlineformat</span><span class="sxs-lookup"><span data-stu-id="2943a-101">Update chartlineformat</span></span>

<span data-ttu-id="2943a-102">Atualiza as propriedades do objeto chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="2943a-102">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2943a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2943a-103">Permissions</span></span>
<span data-ttu-id="2943a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2943a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2943a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2943a-106">Permission type</span></span>      | <span data-ttu-id="2943a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2943a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2943a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2943a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2943a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2943a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2943a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2943a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2943a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2943a-111">Not supported.</span></span>    |
|<span data-ttu-id="2943a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2943a-112">Application</span></span> | <span data-ttu-id="2943a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2943a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2943a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2943a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="2943a-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2943a-115">Optional request headers</span></span>
| <span data-ttu-id="2943a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2943a-116">Name</span></span>       | <span data-ttu-id="2943a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2943a-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2943a-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2943a-118">Authorization</span></span>  | <span data-ttu-id="2943a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2943a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2943a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2943a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2943a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2943a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2943a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2943a-124">Request body</span></span>
<span data-ttu-id="2943a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2943a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2943a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2943a-128">Property</span></span>     | <span data-ttu-id="2943a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2943a-129">Type</span></span>   |<span data-ttu-id="2943a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2943a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2943a-131">color</span><span class="sxs-lookup"><span data-stu-id="2943a-131">color</span></span>|<span data-ttu-id="2943a-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2943a-132">string</span></span>|<span data-ttu-id="2943a-133">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="2943a-133">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="2943a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2943a-134">Response</span></span>

<span data-ttu-id="2943a-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartLineFormat](../resources/chartlineformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2943a-135">If successful, this method returns a `200 OK` response code and updated [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2943a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2943a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2943a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2943a-137">Request</span></span>
<span data-ttu-id="2943a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2943a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="2943a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2943a-139">Response</span></span>
<span data-ttu-id="2943a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2943a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
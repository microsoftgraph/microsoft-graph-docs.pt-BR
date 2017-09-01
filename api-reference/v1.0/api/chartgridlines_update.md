# <a name="update-chartgridlines"></a><span data-ttu-id="93c75-101">Atualizar chartgridlines</span><span class="sxs-lookup"><span data-stu-id="93c75-101">Update chartgridlines</span></span>

<span data-ttu-id="93c75-102">Atualiza as propriedades do objeto chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="93c75-102">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="93c75-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="93c75-103">Permissions</span></span>
<span data-ttu-id="93c75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="93c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="93c75-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93c75-106">Permission type</span></span>      | <span data-ttu-id="93c75-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93c75-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93c75-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93c75-108">Delegated (work or school account)</span></span> | <span data-ttu-id="93c75-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93c75-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="93c75-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93c75-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93c75-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93c75-111">Not supported.</span></span>    |
|<span data-ttu-id="93c75-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93c75-112">Application</span></span> | <span data-ttu-id="93c75-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93c75-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93c75-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93c75-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/minorgridlines
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/majorgridlines
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines
```
## <a name="optional-request-headers"></a><span data-ttu-id="93c75-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="93c75-115">Optional request headers</span></span>
| <span data-ttu-id="93c75-116">Nome</span><span class="sxs-lookup"><span data-stu-id="93c75-116">Name</span></span>       | <span data-ttu-id="93c75-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="93c75-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="93c75-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="93c75-118">Authorization</span></span>  | <span data-ttu-id="93c75-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93c75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93c75-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93c75-121">Request body</span></span>
<span data-ttu-id="93c75-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="93c75-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="93c75-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93c75-125">Property</span></span>     | <span data-ttu-id="93c75-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="93c75-126">Type</span></span>   |<span data-ttu-id="93c75-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="93c75-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93c75-128">visible</span><span class="sxs-lookup"><span data-stu-id="93c75-128">visible</span></span>|<span data-ttu-id="93c75-129">booliano</span><span class="sxs-lookup"><span data-stu-id="93c75-129">boolean</span></span>|<span data-ttu-id="93c75-130">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="93c75-130">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="93c75-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="93c75-131">Response</span></span>

<span data-ttu-id="93c75-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartGridlines](../resources/chartgridlines.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93c75-132">If successful, this method returns a `200 OK` response code and updated [ChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93c75-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93c75-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93c75-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93c75-134">Request</span></span>
<span data-ttu-id="93c75-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93c75-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/minorgridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="93c75-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="93c75-136">Response</span></span>
<span data-ttu-id="93c75-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93c75-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartGridLines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
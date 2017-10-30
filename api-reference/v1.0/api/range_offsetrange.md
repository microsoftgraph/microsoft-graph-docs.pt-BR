# <a name="range-offsetrange"></a><span data-ttu-id="e10a6-101">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="e10a6-101">Range: OffsetRange</span></span>

<span data-ttu-id="e10a6-p101">Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.</span><span class="sxs-lookup"><span data-stu-id="e10a6-p101">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="e10a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e10a6-105">Permissions</span></span>
<span data-ttu-id="e10a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e10a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e10a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e10a6-108">Permission type</span></span>      | <span data-ttu-id="e10a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e10a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e10a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e10a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e10a6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e10a6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e10a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e10a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e10a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e10a6-113">Not supported.</span></span>    |
|<span data-ttu-id="e10a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e10a6-114">Application</span></span> | <span data-ttu-id="e10a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e10a6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e10a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e10a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="e10a6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e10a6-117">Request headers</span></span>
| <span data-ttu-id="e10a6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e10a6-118">Name</span></span>       | <span data-ttu-id="e10a6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e10a6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e10a6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e10a6-120">Authorization</span></span>  | <span data-ttu-id="e10a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e10a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e10a6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e10a6-123">Request body</span></span>
<span data-ttu-id="e10a6-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e10a6-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e10a6-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e10a6-125">Parameter</span></span>    | <span data-ttu-id="e10a6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e10a6-126">Type</span></span>   |<span data-ttu-id="e10a6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e10a6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e10a6-128">rowOffset</span><span class="sxs-lookup"><span data-stu-id="e10a6-128">rowOffset</span></span>|<span data-ttu-id="e10a6-129">number</span><span class="sxs-lookup"><span data-stu-id="e10a6-129">number</span></span>|<span data-ttu-id="e10a6-p104">O número de linhas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para baixo e os negativos, para cima.</span><span class="sxs-lookup"><span data-stu-id="e10a6-p104">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="e10a6-132">columnOffset</span><span class="sxs-lookup"><span data-stu-id="e10a6-132">columnOffset</span></span>|<span data-ttu-id="e10a6-133">number</span><span class="sxs-lookup"><span data-stu-id="e10a6-133">number</span></span>|<span data-ttu-id="e10a6-p105">O número de colunas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para a direita e os negativos, para a esquerda.</span><span class="sxs-lookup"><span data-stu-id="e10a6-p105">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="e10a6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e10a6-136">Response</span></span>

<span data-ttu-id="e10a6-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e10a6-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e10a6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e10a6-138">Example</span></span>
<span data-ttu-id="e10a6-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e10a6-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e10a6-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e10a6-140">Request</span></span>
<span data-ttu-id="e10a6-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e10a6-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="e10a6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e10a6-142">Response</span></span>
<span data-ttu-id="e10a6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e10a6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
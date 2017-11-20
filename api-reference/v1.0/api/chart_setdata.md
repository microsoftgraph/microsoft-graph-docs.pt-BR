# <a name="chart-setdata"></a><span data-ttu-id="f028c-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="f028c-101">Chart: setData</span></span>

<span data-ttu-id="f028c-102">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f028c-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f028c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f028c-103">Permissions</span></span>
<span data-ttu-id="f028c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f028c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f028c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f028c-106">Permission type</span></span>      | <span data-ttu-id="f028c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f028c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f028c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f028c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f028c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f028c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f028c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f028c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f028c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f028c-111">Not supported.</span></span>    |
|<span data-ttu-id="f028c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f028c-112">Application</span></span> | <span data-ttu-id="f028c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f028c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f028c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f028c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="f028c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f028c-115">Request headers</span></span>
| <span data-ttu-id="f028c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f028c-116">Name</span></span>       | <span data-ttu-id="f028c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f028c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f028c-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="f028c-118">Authorization</span></span>  | <span data-ttu-id="f028c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f028c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f028c-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f028c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f028c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f028c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f028c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f028c-124">Request body</span></span>
<span data-ttu-id="f028c-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028c-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f028c-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f028c-126">Parameter</span></span>    | <span data-ttu-id="f028c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f028c-127">Type</span></span>   |<span data-ttu-id="f028c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f028c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f028c-129">sourceData</span><span class="sxs-lookup"><span data-stu-id="f028c-129">sourceData</span></span>|<span data-ttu-id="f028c-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f028c-130">string</span></span>|<span data-ttu-id="f028c-131">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="f028c-131">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="f028c-132">seriesBy</span><span class="sxs-lookup"><span data-stu-id="f028c-132">seriesBy</span></span>|<span data-ttu-id="f028c-133">string</span><span class="sxs-lookup"><span data-stu-id="f028c-133">string</span></span>|<span data-ttu-id="f028c-p104">Opcional. Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico. Pode ser um dos seguintes: automático (padrão), linhas ou colunas.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="f028c-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="f028c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028c-138">Response</span></span>

<span data-ttu-id="f028c-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f028c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f028c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f028c-141">Example</span></span>
<span data-ttu-id="f028c-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f028c-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f028c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f028c-143">Request</span></span>
<span data-ttu-id="f028c-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028c-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="f028c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028c-145">Response</span></span>
<span data-ttu-id="f028c-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f028c-146">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
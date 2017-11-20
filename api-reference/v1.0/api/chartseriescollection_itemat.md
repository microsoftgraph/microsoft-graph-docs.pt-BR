# <a name="chartseriescollection-itemat"></a><span data-ttu-id="77e2a-101">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="77e2a-101">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="77e2a-102">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="77e2a-102">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="77e2a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="77e2a-103">Permissions</span></span>
<span data-ttu-id="77e2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="77e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="77e2a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77e2a-106">Permission type</span></span>      | <span data-ttu-id="77e2a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77e2a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77e2a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77e2a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="77e2a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77e2a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77e2a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77e2a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77e2a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77e2a-111">Not supported.</span></span>    |
|<span data-ttu-id="77e2a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77e2a-112">Application</span></span> | <span data-ttu-id="77e2a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77e2a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77e2a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77e2a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="77e2a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77e2a-115">Request headers</span></span>
| <span data-ttu-id="77e2a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="77e2a-116">Name</span></span>       | <span data-ttu-id="77e2a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="77e2a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77e2a-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="77e2a-118">Authorization</span></span>  | <span data-ttu-id="77e2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77e2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77e2a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="77e2a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="77e2a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="77e2a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77e2a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77e2a-124">Request body</span></span>
<span data-ttu-id="77e2a-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77e2a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77e2a-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77e2a-126">Parameter</span></span>    | <span data-ttu-id="77e2a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="77e2a-127">Type</span></span>   |<span data-ttu-id="77e2a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="77e2a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77e2a-129">index</span><span class="sxs-lookup"><span data-stu-id="77e2a-129">index</span></span>|<span data-ttu-id="77e2a-130">number</span><span class="sxs-lookup"><span data-stu-id="77e2a-130">number</span></span>|<span data-ttu-id="77e2a-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="77e2a-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="77e2a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="77e2a-133">Response</span></span>

<span data-ttu-id="77e2a-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77e2a-134">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77e2a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77e2a-135">Example</span></span>
<span data-ttu-id="77e2a-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="77e2a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="77e2a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77e2a-137">Request</span></span>
<span data-ttu-id="77e2a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77e2a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="77e2a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77e2a-139">Response</span></span>
<span data-ttu-id="77e2a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77e2a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
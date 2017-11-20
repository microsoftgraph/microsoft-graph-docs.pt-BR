# <a name="chartcollection-itemat"></a><span data-ttu-id="dbde4-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="dbde4-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="dbde4-102">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="dbde4-102">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbde4-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbde4-103">Permissions</span></span>
<span data-ttu-id="dbde4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dbde4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dbde4-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbde4-106">Permission type</span></span>      | <span data-ttu-id="dbde4-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbde4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbde4-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbde4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dbde4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbde4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbde4-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbde4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbde4-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbde4-111">Not supported.</span></span>    |
|<span data-ttu-id="dbde4-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbde4-112">Application</span></span> | <span data-ttu-id="dbde4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbde4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbde4-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbde4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="dbde4-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbde4-115">Request headers</span></span>
| <span data-ttu-id="dbde4-116">Nome</span><span class="sxs-lookup"><span data-stu-id="dbde4-116">Name</span></span>       | <span data-ttu-id="dbde4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbde4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dbde4-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbde4-118">Authorization</span></span>  | <span data-ttu-id="dbde4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbde4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbde4-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dbde4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="dbde4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dbde4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbde4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbde4-124">Request body</span></span>
<span data-ttu-id="dbde4-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbde4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbde4-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dbde4-126">Parameter</span></span>    | <span data-ttu-id="dbde4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbde4-127">Type</span></span>   |<span data-ttu-id="dbde4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbde4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbde4-129">index</span><span class="sxs-lookup"><span data-stu-id="dbde4-129">index</span></span>|<span data-ttu-id="dbde4-130">number</span><span class="sxs-lookup"><span data-stu-id="dbde4-130">number</span></span>|<span data-ttu-id="dbde4-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="dbde4-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="dbde4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbde4-133">Response</span></span>

<span data-ttu-id="dbde4-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbde4-134">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbde4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbde4-135">Example</span></span>
<span data-ttu-id="dbde4-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dbde4-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dbde4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbde4-137">Request</span></span>
<span data-ttu-id="dbde4-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbde4-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="dbde4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbde4-139">Response</span></span>
<span data-ttu-id="dbde4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbde4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
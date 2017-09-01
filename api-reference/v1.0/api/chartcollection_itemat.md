# <a name="chartcollection-itemat"></a><span data-ttu-id="71386-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="71386-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="71386-102">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="71386-102">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="71386-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="71386-103">Permissions</span></span>
<span data-ttu-id="71386-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71386-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71386-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71386-106">Permission type</span></span>      | <span data-ttu-id="71386-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71386-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71386-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71386-108">Delegated (work or school account)</span></span> | <span data-ttu-id="71386-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71386-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71386-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71386-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71386-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71386-111">Not supported.</span></span>    |
|<span data-ttu-id="71386-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71386-112">Application</span></span> | <span data-ttu-id="71386-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71386-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71386-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71386-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="71386-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71386-115">Request headers</span></span>
| <span data-ttu-id="71386-116">Nome</span><span class="sxs-lookup"><span data-stu-id="71386-116">Name</span></span>       | <span data-ttu-id="71386-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="71386-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71386-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="71386-118">Authorization</span></span>  | <span data-ttu-id="71386-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71386-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71386-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71386-121">Request body</span></span>
<span data-ttu-id="71386-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71386-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71386-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="71386-123">Parameter</span></span>    | <span data-ttu-id="71386-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="71386-124">Type</span></span>   |<span data-ttu-id="71386-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="71386-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71386-126">índice</span><span class="sxs-lookup"><span data-stu-id="71386-126">index</span></span>|<span data-ttu-id="71386-127">number</span><span class="sxs-lookup"><span data-stu-id="71386-127">number</span></span>|<span data-ttu-id="71386-p103">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="71386-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="71386-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="71386-130">Response</span></span>

<span data-ttu-id="71386-131">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71386-131">If successful, this method returns `200, OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71386-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71386-132">Example</span></span>
<span data-ttu-id="71386-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="71386-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71386-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71386-134">Request</span></span>
<span data-ttu-id="71386-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71386-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="71386-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71386-136">Response</span></span>
<span data-ttu-id="71386-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71386-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
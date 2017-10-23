# <a name="chartpointscollection-itemat"></a><span data-ttu-id="7314f-101">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="7314f-101">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="7314f-102">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="7314f-102">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="7314f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7314f-103">Permissions</span></span>
<span data-ttu-id="7314f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7314f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7314f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7314f-106">Permission type</span></span>      | <span data-ttu-id="7314f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7314f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7314f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7314f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7314f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7314f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7314f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7314f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7314f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7314f-111">Not supported.</span></span>    |
|<span data-ttu-id="7314f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7314f-112">Application</span></span> | <span data-ttu-id="7314f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7314f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7314f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7314f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="7314f-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7314f-115">Request headers</span></span>
| <span data-ttu-id="7314f-116">Nome</span><span class="sxs-lookup"><span data-stu-id="7314f-116">Name</span></span>       | <span data-ttu-id="7314f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="7314f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7314f-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="7314f-118">Authorization</span></span>  | <span data-ttu-id="7314f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7314f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7314f-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7314f-121">Request body</span></span>
<span data-ttu-id="7314f-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7314f-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7314f-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7314f-123">Parameter</span></span>    | <span data-ttu-id="7314f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7314f-124">Type</span></span>   |<span data-ttu-id="7314f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7314f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7314f-126">índice</span><span class="sxs-lookup"><span data-stu-id="7314f-126">index</span></span>|<span data-ttu-id="7314f-127">number</span><span class="sxs-lookup"><span data-stu-id="7314f-127">number</span></span>|<span data-ttu-id="7314f-p103">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="7314f-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7314f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7314f-130">Response</span></span>

<span data-ttu-id="7314f-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartPoint](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7314f-131">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7314f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7314f-132">Example</span></span>
<span data-ttu-id="7314f-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7314f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7314f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7314f-134">Request</span></span>
<span data-ttu-id="7314f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7314f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="7314f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7314f-136">Response</span></span>
<span data-ttu-id="7314f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7314f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
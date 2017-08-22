# <a name="rangebordercollection-itemat"></a><span data-ttu-id="fbc0d-101">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="fbc0d-101">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="fbc0d-102">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-102">Gets a border object using its index</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbc0d-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbc0d-103">Prerequisites</span></span>
<span data-ttu-id="fbc0d-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="fbc0d-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="fbc0d-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbc0d-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="fbc0d-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbc0d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="fbc0d-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc0d-107">Request headers</span></span>
| <span data-ttu-id="fbc0d-108">Nome</span><span class="sxs-lookup"><span data-stu-id="fbc0d-108">Name</span></span>       | <span data-ttu-id="fbc0d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc0d-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fbc0d-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbc0d-110">Authorization</span></span>  | <span data-ttu-id="fbc0d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="fbc0d-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc0d-113">Request body</span></span>
<span data-ttu-id="fbc0d-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fbc0d-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fbc0d-115">Parameter</span></span>    | <span data-ttu-id="fbc0d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc0d-116">Type</span></span>   |<span data-ttu-id="fbc0d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc0d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbc0d-118">índice</span><span class="sxs-lookup"><span data-stu-id="fbc0d-118">index</span></span>|<span data-ttu-id="fbc0d-119">number</span><span class="sxs-lookup"><span data-stu-id="fbc0d-119">number</span></span>|<span data-ttu-id="fbc0d-p102">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-p102">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="fbc0d-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc0d-122">Response</span></span>

<span data-ttu-id="fbc0d-123">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [RangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-123">If successful, this method returns `200, OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc0d-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbc0d-124">Example</span></span>
<span data-ttu-id="fbc0d-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fbc0d-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc0d-126">Request</span></span>
<span data-ttu-id="fbc0d-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="fbc0d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc0d-128">Response</span></span>
<span data-ttu-id="fbc0d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbc0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
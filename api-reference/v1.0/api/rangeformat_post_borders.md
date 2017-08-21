# <a name="create-rangeborder"></a><span data-ttu-id="63482-101">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="63482-101">Create RangeBorder</span></span>

<span data-ttu-id="63482-102">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="63482-102">Use this API to create a new RangeBorder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63482-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63482-103">Prerequisites</span></span>
<span data-ttu-id="63482-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="63482-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="63482-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63482-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="63482-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63482-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="63482-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63482-107">Request headers</span></span>
| <span data-ttu-id="63482-108">Nome</span><span class="sxs-lookup"><span data-stu-id="63482-108">Name</span></span>       | <span data-ttu-id="63482-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="63482-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63482-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="63482-110">Authorization</span></span>  | <span data-ttu-id="63482-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63482-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="63482-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63482-113">Request body</span></span>
<span data-ttu-id="63482-114">No corpo da solicitação, forneça uma representação JSON do objeto [RangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="63482-114">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="63482-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="63482-115">Response</span></span>

<span data-ttu-id="63482-116">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [RangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63482-116">If successful, this method returns `201, Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63482-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63482-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63482-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63482-118">Request</span></span>
<span data-ttu-id="63482-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63482-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
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
<span data-ttu-id="63482-120">No corpo da solicitação, forneça uma representação JSON do objeto [RangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="63482-120">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="63482-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="63482-121">Response</span></span>
<span data-ttu-id="63482-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63482-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
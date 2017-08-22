# <a name="range-merge"></a><span data-ttu-id="08a7d-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="08a7d-101">Range: merge</span></span>

<span data-ttu-id="08a7d-102">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="08a7d-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08a7d-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08a7d-103">Prerequisites</span></span>
<span data-ttu-id="08a7d-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="08a7d-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="08a7d-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08a7d-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="08a7d-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08a7d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(<address>)/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="08a7d-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08a7d-107">Request headers</span></span>
| <span data-ttu-id="08a7d-108">Nome</span><span class="sxs-lookup"><span data-stu-id="08a7d-108">Name</span></span>       | <span data-ttu-id="08a7d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a7d-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08a7d-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="08a7d-110">Authorization</span></span>  | <span data-ttu-id="08a7d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a7d-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="08a7d-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08a7d-113">Request body</span></span>
<span data-ttu-id="08a7d-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a7d-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08a7d-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08a7d-115">Parameter</span></span>    | <span data-ttu-id="08a7d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="08a7d-116">Type</span></span>   |<span data-ttu-id="08a7d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a7d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08a7d-118">across</span><span class="sxs-lookup"><span data-stu-id="08a7d-118">across</span></span>|<span data-ttu-id="08a7d-119">booliano</span><span class="sxs-lookup"><span data-stu-id="08a7d-119">boolean</span></span>|<span data-ttu-id="08a7d-p102">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="08a7d-p102">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="08a7d-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a7d-123">Response</span></span>

<span data-ttu-id="08a7d-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a7d-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08a7d-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08a7d-126">Example</span></span>
<span data-ttu-id="08a7d-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="08a7d-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08a7d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08a7d-128">Request</span></span>
<span data-ttu-id="08a7d-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a7d-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="08a7d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a7d-130">Response</span></span>
<span data-ttu-id="08a7d-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a7d-131">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
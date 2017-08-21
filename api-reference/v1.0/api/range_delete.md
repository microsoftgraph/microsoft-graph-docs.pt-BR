# <a name="range-delete"></a><span data-ttu-id="1db16-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="1db16-101">Range: delete</span></span>

<span data-ttu-id="1db16-102">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="1db16-102">Deletes the cells associated with the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1db16-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1db16-103">Prerequisites</span></span>
<span data-ttu-id="1db16-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="1db16-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="1db16-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1db16-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="1db16-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1db16-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="1db16-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1db16-107">Request headers</span></span>
| <span data-ttu-id="1db16-108">Nome</span><span class="sxs-lookup"><span data-stu-id="1db16-108">Name</span></span>       | <span data-ttu-id="1db16-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1db16-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1db16-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="1db16-110">Authorization</span></span>  | <span data-ttu-id="1db16-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1db16-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1db16-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1db16-113">Request body</span></span>
<span data-ttu-id="1db16-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1db16-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1db16-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1db16-115">Parameter</span></span>    | <span data-ttu-id="1db16-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="1db16-116">Type</span></span>   |<span data-ttu-id="1db16-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="1db16-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1db16-118">shift</span><span class="sxs-lookup"><span data-stu-id="1db16-118">shift</span></span>|<span data-ttu-id="1db16-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1db16-119">string</span></span>|<span data-ttu-id="1db16-p102">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="1db16-p102">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="1db16-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1db16-122">Response</span></span>

<span data-ttu-id="1db16-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1db16-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1db16-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1db16-125">Example</span></span>
<span data-ttu-id="1db16-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1db16-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1db16-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1db16-127">Request</span></span>
<span data-ttu-id="1db16-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1db16-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="1db16-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1db16-129">Response</span></span>
<span data-ttu-id="1db16-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1db16-130">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
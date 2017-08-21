# <a name="rangesort-apply"></a><span data-ttu-id="f7374-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="f7374-101">RangeSort: apply</span></span>

<span data-ttu-id="f7374-102">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="f7374-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7374-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7374-103">Prerequisites</span></span>
<span data-ttu-id="f7374-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="f7374-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="f7374-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7374-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="f7374-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7374-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="f7374-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7374-107">Request headers</span></span>
| <span data-ttu-id="f7374-108">Nome</span><span class="sxs-lookup"><span data-stu-id="f7374-108">Name</span></span>       | <span data-ttu-id="f7374-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7374-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7374-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7374-110">Authorization</span></span>  | <span data-ttu-id="f7374-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7374-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f7374-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7374-113">Request body</span></span>
<span data-ttu-id="f7374-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7374-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7374-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f7374-115">Parameter</span></span>    | <span data-ttu-id="f7374-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7374-116">Type</span></span>   |<span data-ttu-id="f7374-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7374-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7374-118">campos</span><span class="sxs-lookup"><span data-stu-id="f7374-118">fields</span></span>|<span data-ttu-id="f7374-119">SortField</span><span class="sxs-lookup"><span data-stu-id="f7374-119">SortField</span></span>|<span data-ttu-id="f7374-120">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="f7374-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="f7374-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="f7374-121">matchCase</span></span>|<span data-ttu-id="f7374-122">booliano</span><span class="sxs-lookup"><span data-stu-id="f7374-122">boolean</span></span>|<span data-ttu-id="f7374-p102">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="f7374-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="f7374-125">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="f7374-125">hasHeaders</span></span>|<span data-ttu-id="f7374-126">booliano</span><span class="sxs-lookup"><span data-stu-id="f7374-126">boolean</span></span>|<span data-ttu-id="f7374-p103">Opcional. Se o intervalo tem um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="f7374-p103">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="f7374-129">orientation</span><span class="sxs-lookup"><span data-stu-id="f7374-129">orientation</span></span>|<span data-ttu-id="f7374-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7374-130">string</span></span>|<span data-ttu-id="f7374-p104">Opcional. Se a operação classifica linhas ou colunas.  Os valores possíveis são: `Rows` e `Columns`.</span><span class="sxs-lookup"><span data-stu-id="f7374-p104">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="f7374-134">method</span><span class="sxs-lookup"><span data-stu-id="f7374-134">method</span></span>|<span data-ttu-id="f7374-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7374-135">string</span></span>|<span data-ttu-id="f7374-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="f7374-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="f7374-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7374-139">Response</span></span>

<span data-ttu-id="f7374-p106">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7374-p106">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7374-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7374-142">Example</span></span>
<span data-ttu-id="f7374-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f7374-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7374-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7374-144">Request</span></span>
<span data-ttu-id="f7374-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7374-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="f7374-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7374-146">Response</span></span>
<span data-ttu-id="f7374-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7374-147">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
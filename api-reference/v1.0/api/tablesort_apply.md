# <a name="tablesort-apply"></a><span data-ttu-id="2d479-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="2d479-101">TableSort: apply</span></span>

<span data-ttu-id="2d479-102">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="2d479-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d479-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d479-103">Prerequisites</span></span>
<span data-ttu-id="2d479-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="2d479-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="2d479-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d479-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="2d479-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d479-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="2d479-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d479-107">Request headers</span></span>
| <span data-ttu-id="2d479-108">Nome</span><span class="sxs-lookup"><span data-stu-id="2d479-108">Name</span></span>       | <span data-ttu-id="2d479-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d479-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d479-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d479-110">Authorization</span></span>  | <span data-ttu-id="2d479-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d479-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2d479-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d479-113">Request body</span></span>
<span data-ttu-id="2d479-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d479-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d479-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2d479-115">Parameter</span></span>    | <span data-ttu-id="2d479-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d479-116">Type</span></span>   |<span data-ttu-id="2d479-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d479-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d479-118">campos</span><span class="sxs-lookup"><span data-stu-id="2d479-118">fields</span></span>|<span data-ttu-id="2d479-119">SortField</span><span class="sxs-lookup"><span data-stu-id="2d479-119">SortField</span></span>|<span data-ttu-id="2d479-120">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="2d479-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="2d479-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="2d479-121">matchCase</span></span>|<span data-ttu-id="2d479-122">booliano</span><span class="sxs-lookup"><span data-stu-id="2d479-122">boolean</span></span>|<span data-ttu-id="2d479-p102">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="2d479-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="2d479-125">method</span><span class="sxs-lookup"><span data-stu-id="2d479-125">method</span></span>|<span data-ttu-id="2d479-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d479-126">string</span></span>|<span data-ttu-id="2d479-p103">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="2d479-p103">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="2d479-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d479-130">Response</span></span>

<span data-ttu-id="2d479-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d479-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d479-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d479-133">Example</span></span>
<span data-ttu-id="2d479-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2d479-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d479-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d479-135">Request</span></span>
<span data-ttu-id="2d479-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d479-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

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
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="2d479-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d479-137">Response</span></span>
<span data-ttu-id="2d479-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d479-138">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="filter-apply"></a><span data-ttu-id="79b6c-101">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="79b6c-101">Filter: apply</span></span>

<span data-ttu-id="79b6c-102">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="79b6c-102">Apply the given filter criteria on the given column.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79b6c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79b6c-103">Prerequisites</span></span>
<span data-ttu-id="79b6c-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="79b6c-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="79b6c-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b6c-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="79b6c-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79b6c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="79b6c-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79b6c-107">Request headers</span></span>
| <span data-ttu-id="79b6c-108">Nome</span><span class="sxs-lookup"><span data-stu-id="79b6c-108">Name</span></span>       | <span data-ttu-id="79b6c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79b6c-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79b6c-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="79b6c-110">Authorization</span></span>  | <span data-ttu-id="79b6c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79b6c-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="79b6c-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79b6c-113">Request body</span></span>
<span data-ttu-id="79b6c-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79b6c-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79b6c-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="79b6c-115">Parameter</span></span>    | <span data-ttu-id="79b6c-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="79b6c-116">Type</span></span>   |<span data-ttu-id="79b6c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="79b6c-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79b6c-118">critérios</span><span class="sxs-lookup"><span data-stu-id="79b6c-118">criteria</span></span>|<span data-ttu-id="79b6c-119">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="79b6c-119">FilterCriteria</span></span>|<span data-ttu-id="79b6c-120">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="79b6c-120">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="79b6c-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b6c-121">Response</span></span>

<span data-ttu-id="79b6c-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79b6c-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b6c-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79b6c-124">Example</span></span>
<span data-ttu-id="79b6c-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="79b6c-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79b6c-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79b6c-126">Request</span></span>
<span data-ttu-id="79b6c-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79b6c-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="79b6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b6c-128">Response</span></span>
<span data-ttu-id="79b6c-129">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79b6c-129">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
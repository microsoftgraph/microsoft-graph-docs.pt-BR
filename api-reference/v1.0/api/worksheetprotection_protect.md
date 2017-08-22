# <a name="worksheetprotection-protect"></a><span data-ttu-id="24c67-101">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="24c67-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="24c67-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="24c67-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24c67-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24c67-104">Prerequisites</span></span>
<span data-ttu-id="24c67-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="24c67-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="24c67-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24c67-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="24c67-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24c67-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="24c67-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24c67-108">Request headers</span></span>
| <span data-ttu-id="24c67-109">Nome</span><span class="sxs-lookup"><span data-stu-id="24c67-109">Name</span></span>       | <span data-ttu-id="24c67-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="24c67-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24c67-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="24c67-111">Authorization</span></span>  | <span data-ttu-id="24c67-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24c67-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="24c67-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24c67-114">Request body</span></span>
<span data-ttu-id="24c67-115">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24c67-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24c67-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="24c67-116">Parameter</span></span>    | <span data-ttu-id="24c67-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="24c67-117">Type</span></span>   |<span data-ttu-id="24c67-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="24c67-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24c67-119">opções</span><span class="sxs-lookup"><span data-stu-id="24c67-119">options</span></span>|<span data-ttu-id="24c67-120">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="24c67-120">WorksheetProtectionOptions</span></span>|<span data-ttu-id="24c67-p103">Opcional. Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="24c67-p103">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="24c67-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c67-123">Response</span></span>

<span data-ttu-id="24c67-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24c67-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c67-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24c67-126">Example</span></span>
<span data-ttu-id="24c67-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="24c67-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24c67-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24c67-128">Request</span></span>
<span data-ttu-id="24c67-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24c67-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="24c67-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c67-130">Response</span></span>
<span data-ttu-id="24c67-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24c67-131">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

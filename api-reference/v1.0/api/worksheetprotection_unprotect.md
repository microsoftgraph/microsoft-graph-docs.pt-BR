# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="46b5c-101">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="46b5c-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="46b5c-102">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="46b5c-102">Unprotect a worksheet</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46b5c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46b5c-103">Prerequisites</span></span>
<span data-ttu-id="46b5c-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="46b5c-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="46b5c-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b5c-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="46b5c-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46b5c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="46b5c-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46b5c-107">Request headers</span></span>
| <span data-ttu-id="46b5c-108">Nome</span><span class="sxs-lookup"><span data-stu-id="46b5c-108">Name</span></span>       | <span data-ttu-id="46b5c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b5c-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46b5c-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="46b5c-110">Authorization</span></span>  | <span data-ttu-id="46b5c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46b5c-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="46b5c-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46b5c-113">Request body</span></span>
<span data-ttu-id="46b5c-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b5c-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46b5c-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46b5c-115">Parameter</span></span>    | <span data-ttu-id="46b5c-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="46b5c-116">Type</span></span>   |<span data-ttu-id="46b5c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b5c-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46b5c-118">password</span><span class="sxs-lookup"><span data-stu-id="46b5c-118">password</span></span>|<span data-ttu-id="46b5c-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46b5c-119">string</span></span>|<span data-ttu-id="46b5c-p102">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="46b5c-p102">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="46b5c-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b5c-122">Response</span></span>

<span data-ttu-id="46b5c-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b5c-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b5c-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46b5c-125">Example</span></span>
<span data-ttu-id="46b5c-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="46b5c-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46b5c-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46b5c-127">Request</span></span>
<span data-ttu-id="46b5c-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b5c-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="46b5c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b5c-129">Response</span></span>
<span data-ttu-id="46b5c-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b5c-130">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
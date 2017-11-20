# <a name="worksheetprotection-protect"></a><span data-ttu-id="cc7c0-101">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="cc7c0-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="cc7c0-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc7c0-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc7c0-104">Permissions</span></span>
<span data-ttu-id="cc7c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc7c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc7c0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc7c0-107">Permission type</span></span>      | <span data-ttu-id="cc7c0-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc7c0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc7c0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc7c0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="cc7c0-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc7c0-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cc7c0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc7c0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc7c0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-112">Not supported.</span></span>    |
|<span data-ttu-id="cc7c0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc7c0-113">Application</span></span> | <span data-ttu-id="cc7c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc7c0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc7c0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="cc7c0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc7c0-116">Request headers</span></span>
| <span data-ttu-id="cc7c0-117">Nome</span><span class="sxs-lookup"><span data-stu-id="cc7c0-117">Name</span></span>       | <span data-ttu-id="cc7c0-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc7c0-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc7c0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc7c0-119">Authorization</span></span>  | <span data-ttu-id="cc7c0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc7c0-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cc7c0-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="cc7c0-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc7c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc7c0-125">Request body</span></span>
<span data-ttu-id="cc7c0-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc7c0-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cc7c0-127">Parameter</span></span>    | <span data-ttu-id="cc7c0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc7c0-128">Type</span></span>   |<span data-ttu-id="cc7c0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc7c0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc7c0-130">opções</span><span class="sxs-lookup"><span data-stu-id="cc7c0-130">options</span></span>|<span data-ttu-id="cc7c0-131">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="cc7c0-131">WorksheetProtectionOptions</span></span>|<span data-ttu-id="cc7c0-p105">Opcional. Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-p105">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="cc7c0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc7c0-134">Response</span></span>

<span data-ttu-id="cc7c0-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc7c0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc7c0-137">Example</span></span>
<span data-ttu-id="cc7c0-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc7c0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc7c0-139">Request</span></span>
<span data-ttu-id="cc7c0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cc7c0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc7c0-141">Response</span></span>
<span data-ttu-id="cc7c0-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc7c0-142">Here is an example of the response.</span></span> 
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

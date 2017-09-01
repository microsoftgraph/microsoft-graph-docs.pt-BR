# <a name="worksheetprotection-protect"></a><span data-ttu-id="76747-101">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="76747-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="76747-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="76747-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="76747-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="76747-104">Permissions</span></span>
<span data-ttu-id="76747-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76747-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76747-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76747-107">Permission type</span></span>      | <span data-ttu-id="76747-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76747-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76747-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76747-109">Delegated (work or school account)</span></span> | <span data-ttu-id="76747-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76747-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="76747-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76747-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76747-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76747-112">Not supported.</span></span>    |
|<span data-ttu-id="76747-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76747-113">Application</span></span> | <span data-ttu-id="76747-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76747-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76747-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76747-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="76747-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76747-116">Request headers</span></span>
| <span data-ttu-id="76747-117">Nome</span><span class="sxs-lookup"><span data-stu-id="76747-117">Name</span></span>       | <span data-ttu-id="76747-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="76747-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76747-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="76747-119">Authorization</span></span>  | <span data-ttu-id="76747-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76747-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76747-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76747-122">Request body</span></span>
<span data-ttu-id="76747-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76747-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76747-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76747-124">Parameter</span></span>    | <span data-ttu-id="76747-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="76747-125">Type</span></span>   |<span data-ttu-id="76747-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="76747-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76747-127">opções</span><span class="sxs-lookup"><span data-stu-id="76747-127">options</span></span>|<span data-ttu-id="76747-128">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="76747-128">WorksheetProtectionOptions</span></span>|<span data-ttu-id="76747-p104">Opcional. Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="76747-p104">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="76747-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="76747-131">Response</span></span>

<span data-ttu-id="76747-p105">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76747-p105">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76747-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76747-134">Example</span></span>
<span data-ttu-id="76747-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="76747-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76747-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76747-136">Request</span></span>
<span data-ttu-id="76747-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76747-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="76747-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="76747-138">Response</span></span>
<span data-ttu-id="76747-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76747-139">Here is an example of the response.</span></span> 
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

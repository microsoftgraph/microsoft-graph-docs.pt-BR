# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="255f0-101">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="255f0-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="255f0-102">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="255f0-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="255f0-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="255f0-103">Permissions</span></span>
<span data-ttu-id="255f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="255f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="255f0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="255f0-106">Permission type</span></span>      | <span data-ttu-id="255f0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="255f0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="255f0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="255f0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="255f0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="255f0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="255f0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="255f0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="255f0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="255f0-111">Not supported.</span></span>    |
|<span data-ttu-id="255f0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="255f0-112">Application</span></span> | <span data-ttu-id="255f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="255f0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="255f0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="255f0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="255f0-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="255f0-115">Request headers</span></span>
| <span data-ttu-id="255f0-116">Nome</span><span class="sxs-lookup"><span data-stu-id="255f0-116">Name</span></span>       | <span data-ttu-id="255f0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="255f0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="255f0-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="255f0-118">Authorization</span></span>  | <span data-ttu-id="255f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="255f0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="255f0-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="255f0-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="255f0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="255f0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="255f0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="255f0-124">Request body</span></span>
<span data-ttu-id="255f0-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="255f0-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="255f0-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="255f0-126">Parameter</span></span>    | <span data-ttu-id="255f0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="255f0-127">Type</span></span>   |<span data-ttu-id="255f0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="255f0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="255f0-129">senha</span><span class="sxs-lookup"><span data-stu-id="255f0-129">password</span></span>|<span data-ttu-id="255f0-130">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="255f0-130">string</span></span>|<span data-ttu-id="255f0-p104">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="255f0-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="255f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="255f0-133">Response</span></span>

<span data-ttu-id="255f0-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="255f0-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="255f0-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="255f0-136">Example</span></span>
<span data-ttu-id="255f0-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="255f0-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="255f0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="255f0-138">Request</span></span>
<span data-ttu-id="255f0-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="255f0-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="255f0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="255f0-140">Response</span></span>
<span data-ttu-id="255f0-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="255f0-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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
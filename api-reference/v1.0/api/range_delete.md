# <a name="range-delete"></a><span data-ttu-id="6cfe5-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="6cfe5-101">Range: delete</span></span>

<span data-ttu-id="6cfe5-102">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="6cfe5-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cfe5-103">Permissions</span></span>
<span data-ttu-id="6cfe5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6cfe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6cfe5-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cfe5-106">Permission type</span></span>      | <span data-ttu-id="6cfe5-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cfe5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cfe5-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cfe5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6cfe5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cfe5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6cfe5-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cfe5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cfe5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-111">Not supported.</span></span>    |
|<span data-ttu-id="6cfe5-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cfe5-112">Application</span></span> | <span data-ttu-id="6cfe5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cfe5-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cfe5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="6cfe5-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cfe5-115">Request headers</span></span>
| <span data-ttu-id="6cfe5-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6cfe5-116">Name</span></span>       | <span data-ttu-id="6cfe5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cfe5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6cfe5-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cfe5-118">Authorization</span></span>  | <span data-ttu-id="6cfe5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cfe5-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6cfe5-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6cfe5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cfe5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cfe5-124">Request body</span></span>
<span data-ttu-id="6cfe5-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cfe5-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6cfe5-126">Parameter</span></span>    | <span data-ttu-id="6cfe5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cfe5-127">Type</span></span>   |<span data-ttu-id="6cfe5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cfe5-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cfe5-129">shift</span><span class="sxs-lookup"><span data-stu-id="6cfe5-129">shift</span></span>|<span data-ttu-id="6cfe5-130">string</span><span class="sxs-lookup"><span data-stu-id="6cfe5-130">string</span></span>|<span data-ttu-id="6cfe5-131">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-131">Specifies which way to shift the cells.  Possible values are: Down, Right</span></span>  <span data-ttu-id="6cfe5-132">Os valores possíveis são: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-132">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="6cfe5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cfe5-133">Response</span></span>

<span data-ttu-id="6cfe5-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cfe5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cfe5-136">Example</span></span>
<span data-ttu-id="6cfe5-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6cfe5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cfe5-138">Request</span></span>
<span data-ttu-id="6cfe5-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="6cfe5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cfe5-140">Response</span></span>
<span data-ttu-id="6cfe5-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cfe5-141">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
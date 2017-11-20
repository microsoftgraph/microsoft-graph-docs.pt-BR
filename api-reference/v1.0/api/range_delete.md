# <a name="range-delete"></a><span data-ttu-id="6a860-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="6a860-101">Range: delete</span></span>

<span data-ttu-id="6a860-102">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="6a860-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a860-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a860-103">Permissions</span></span>
<span data-ttu-id="6a860-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a860-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a860-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a860-106">Permission type</span></span>      | <span data-ttu-id="6a860-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a860-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a860-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a860-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6a860-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a860-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a860-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a860-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a860-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a860-111">Not supported.</span></span>    |
|<span data-ttu-id="6a860-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a860-112">Application</span></span> | <span data-ttu-id="6a860-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a860-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a860-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a860-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="6a860-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a860-115">Request headers</span></span>
| <span data-ttu-id="6a860-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6a860-116">Name</span></span>       | <span data-ttu-id="6a860-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a860-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a860-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a860-118">Authorization</span></span>  | <span data-ttu-id="6a860-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a860-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a860-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6a860-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6a860-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6a860-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a860-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a860-124">Request body</span></span>
<span data-ttu-id="6a860-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a860-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6a860-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6a860-126">Parameter</span></span>    | <span data-ttu-id="6a860-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a860-127">Type</span></span>   |<span data-ttu-id="6a860-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a860-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a860-129">shift</span><span class="sxs-lookup"><span data-stu-id="6a860-129">shift</span></span>|<span data-ttu-id="6a860-130">string</span><span class="sxs-lookup"><span data-stu-id="6a860-130">string</span></span>|<span data-ttu-id="6a860-p104">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="6a860-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="6a860-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a860-133">Response</span></span>

<span data-ttu-id="6a860-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a860-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a860-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a860-136">Example</span></span>
<span data-ttu-id="6a860-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6a860-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6a860-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a860-138">Request</span></span>
<span data-ttu-id="6a860-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a860-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6a860-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a860-140">Response</span></span>
<span data-ttu-id="6a860-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a860-141">Here is an example of the response.</span></span> 
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
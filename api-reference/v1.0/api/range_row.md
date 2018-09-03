# <a name="range-row"></a><span data-ttu-id="916e1-101">Range: Row</span><span class="sxs-lookup"><span data-stu-id="916e1-101">Range: Row</span></span>

<span data-ttu-id="916e1-102">Obtém uma linha contida no intervalo.</span><span class="sxs-lookup"><span data-stu-id="916e1-102">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="916e1-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="916e1-103">Permissions</span></span>
<span data-ttu-id="916e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="916e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="916e1-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="916e1-106">Permission type</span></span>      | <span data-ttu-id="916e1-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="916e1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="916e1-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="916e1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="916e1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="916e1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="916e1-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="916e1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="916e1-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916e1-111">Not supported.</span></span>    |
|<span data-ttu-id="916e1-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="916e1-112">Application</span></span> | <span data-ttu-id="916e1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916e1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="916e1-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="916e1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/row
POST /workbook/worksheets/{id|name}/range(address='<address>')/row
POST /workbook/tables/{id|name}/columns/{id|name}/range/row

```
## <a name="request-headers"></a><span data-ttu-id="916e1-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="916e1-115">Request headers</span></span>
| <span data-ttu-id="916e1-116">Nome</span><span class="sxs-lookup"><span data-stu-id="916e1-116">Name</span></span>       | <span data-ttu-id="916e1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="916e1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="916e1-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="916e1-118">Authorization</span></span>  | <span data-ttu-id="916e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="916e1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="916e1-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="916e1-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="916e1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="916e1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="916e1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="916e1-124">Request body</span></span>
<span data-ttu-id="916e1-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="916e1-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="916e1-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="916e1-126">Parameter</span></span>    | <span data-ttu-id="916e1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="916e1-127">Type</span></span>   |<span data-ttu-id="916e1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="916e1-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="916e1-129">row</span><span class="sxs-lookup"><span data-stu-id="916e1-129">row</span></span>|<span data-ttu-id="916e1-130">Int32</span><span class="sxs-lookup"><span data-stu-id="916e1-130">Int32</span></span>|<span data-ttu-id="916e1-p104">O número da linha do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="916e1-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="916e1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="916e1-133">Response</span></span>

<span data-ttu-id="916e1-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916e1-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916e1-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="916e1-135">Example</span></span>
<span data-ttu-id="916e1-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="916e1-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="916e1-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="916e1-137">Request</span></span>
<span data-ttu-id="916e1-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="916e1-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_row",
  "idempotent": true,
  "@type": "requestBodyResourceFor.range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/row
Content-type: application/json
Content-length: 18

{
  "row": 2
}
```

##### <a name="response"></a><span data-ttu-id="916e1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="916e1-139">Response</span></span>
<span data-ttu-id="916e1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="916e1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
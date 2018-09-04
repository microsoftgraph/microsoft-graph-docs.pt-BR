# <a name="worksheet-range"></a><span data-ttu-id="cee79-101">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="cee79-101">Worksheet: Range</span></span>

<span data-ttu-id="cee79-102">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="cee79-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="cee79-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="cee79-103">Permissions</span></span>
<span data-ttu-id="cee79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cee79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cee79-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cee79-106">Permission type</span></span>      | <span data-ttu-id="cee79-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cee79-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cee79-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cee79-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cee79-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cee79-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cee79-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cee79-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee79-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cee79-111">Not supported.</span></span>    |
|<span data-ttu-id="cee79-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cee79-112">Application</span></span> | <span data-ttu-id="cee79-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cee79-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cee79-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cee79-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="cee79-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cee79-115">Request headers</span></span>
| <span data-ttu-id="cee79-116">Nome</span><span class="sxs-lookup"><span data-stu-id="cee79-116">Name</span></span>       | <span data-ttu-id="cee79-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="cee79-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cee79-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="cee79-118">Authorization</span></span>  | <span data-ttu-id="cee79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cee79-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cee79-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cee79-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="cee79-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cee79-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="cee79-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cee79-124">Function parameters</span></span>

| <span data-ttu-id="cee79-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cee79-125">Parameter</span></span>    | <span data-ttu-id="cee79-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="cee79-126">Type</span></span>   |<span data-ttu-id="cee79-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="cee79-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cee79-128">address</span><span class="sxs-lookup"><span data-stu-id="cee79-128">address</span></span>|<span data-ttu-id="cee79-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cee79-129">string</span></span>|<span data-ttu-id="cee79-p104">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="cee79-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="cee79-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cee79-133">Response</span></span>

<span data-ttu-id="cee79-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cee79-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cee79-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cee79-135">Example</span></span>
<span data-ttu-id="cee79-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cee79-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cee79-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cee79-137">Request</span></span>
<span data-ttu-id="cee79-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cee79-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="cee79-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cee79-139">Response</span></span>
<span data-ttu-id="cee79-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cee79-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="cee79-143">Se o parâmetro opcional `address` não for especificado, essa função retorna o intervalo inteiro da planilha.</span><span class="sxs-lookup"><span data-stu-id="cee79-143">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="cee79-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cee79-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="cee79-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cee79-145">Response</span></span>

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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
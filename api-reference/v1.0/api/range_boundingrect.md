# <a name="range-boundingrect"></a><span data-ttu-id="958ee-101">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="958ee-101">Range: BoundingRect</span></span>

<span data-ttu-id="958ee-p101">Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="958ee-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="958ee-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="958ee-104">Permissions</span></span>
<span data-ttu-id="958ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="958ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="958ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="958ee-107">Permission type</span></span>      | <span data-ttu-id="958ee-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="958ee-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="958ee-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="958ee-109">Delegated (work or school account)</span></span> | <span data-ttu-id="958ee-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="958ee-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="958ee-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="958ee-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="958ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="958ee-112">Not supported.</span></span>    |
|<span data-ttu-id="958ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="958ee-113">Application</span></span> | <span data-ttu-id="958ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="958ee-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="958ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="958ee-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(<address>)/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="958ee-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="958ee-116">Request headers</span></span>
| <span data-ttu-id="958ee-117">Nome</span><span class="sxs-lookup"><span data-stu-id="958ee-117">Name</span></span>       | <span data-ttu-id="958ee-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="958ee-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="958ee-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="958ee-119">Authorization</span></span>  | <span data-ttu-id="958ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="958ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="958ee-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="958ee-122">Request body</span></span>
<span data-ttu-id="958ee-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="958ee-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="958ee-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="958ee-124">Parameter</span></span>    | <span data-ttu-id="958ee-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="958ee-125">Type</span></span>   |<span data-ttu-id="958ee-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="958ee-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="958ee-127">anotherRange</span><span class="sxs-lookup"><span data-stu-id="958ee-127">anotherRange</span></span>|<span data-ttu-id="958ee-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="958ee-128">string</span></span>|<span data-ttu-id="958ee-129">O objeto de intervalo, endereço ou nome do intervalo.</span><span class="sxs-lookup"><span data-stu-id="958ee-129">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="958ee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="958ee-130">Response</span></span>

<span data-ttu-id="958ee-131">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="958ee-131">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="958ee-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="958ee-132">Example</span></span>
<span data-ttu-id="958ee-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="958ee-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="958ee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="958ee-134">Request</span></span>
<span data-ttu-id="958ee-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="958ee-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="958ee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="958ee-136">Response</span></span>
<span data-ttu-id="958ee-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="958ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
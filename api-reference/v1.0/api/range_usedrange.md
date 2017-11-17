# <a name="range-usedrange"></a><span data-ttu-id="a6cce-101">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="a6cce-101">Range: UsedRange</span></span>

<span data-ttu-id="a6cce-102">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="a6cce-102">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6cce-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6cce-103">Permissions</span></span>
<span data-ttu-id="a6cce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6cce-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6cce-106">Permission type</span></span>      | <span data-ttu-id="a6cce-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6cce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6cce-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6cce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a6cce-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6cce-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a6cce-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6cce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6cce-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6cce-111">Not supported.</span></span>    |
|<span data-ttu-id="a6cce-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6cce-112">Application</span></span> | <span data-ttu-id="a6cce-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6cce-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6cce-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6cce-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="a6cce-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6cce-115">Request headers</span></span>
| <span data-ttu-id="a6cce-116">Nome</span><span class="sxs-lookup"><span data-stu-id="a6cce-116">Name</span></span>       | <span data-ttu-id="a6cce-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6cce-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a6cce-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6cce-118">Authorization</span></span>  | <span data-ttu-id="a6cce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6cce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6cce-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6cce-121">Request body</span></span>
<span data-ttu-id="a6cce-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6cce-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6cce-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6cce-123">Parameter</span></span>    | <span data-ttu-id="a6cce-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6cce-124">Type</span></span>   |<span data-ttu-id="a6cce-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6cce-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6cce-126">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="a6cce-126">valuesOnly</span></span>|<span data-ttu-id="a6cce-127">booliano</span><span class="sxs-lookup"><span data-stu-id="a6cce-127">boolean</span></span>|<span data-ttu-id="a6cce-p103">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="a6cce-p103">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="a6cce-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6cce-130">Response</span></span>

<span data-ttu-id="a6cce-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6cce-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6cce-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6cce-132">Example</span></span>
<span data-ttu-id="a6cce-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a6cce-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a6cce-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6cce-134">Request</span></span>
<span data-ttu-id="a6cce-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6cce-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a6cce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6cce-136">Response</span></span>
<span data-ttu-id="a6cce-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6cce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="range-intersection"></a><span data-ttu-id="a4ddc-101">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="a4ddc-101">Range: Intersection</span></span>

<span data-ttu-id="a4ddc-102">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4ddc-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4ddc-103">Permissions</span></span>
<span data-ttu-id="a4ddc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a4ddc-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4ddc-106">Permission type</span></span>      | <span data-ttu-id="a4ddc-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4ddc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4ddc-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4ddc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a4ddc-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4ddc-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a4ddc-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4ddc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4ddc-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-111">Not supported.</span></span>    |
|<span data-ttu-id="a4ddc-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4ddc-112">Application</span></span> | <span data-ttu-id="a4ddc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4ddc-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ddc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="a4ddc-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ddc-115">Request headers</span></span>
| <span data-ttu-id="a4ddc-116">Nome</span><span class="sxs-lookup"><span data-stu-id="a4ddc-116">Name</span></span>       | <span data-ttu-id="a4ddc-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4ddc-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4ddc-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4ddc-118">Authorization</span></span>  | <span data-ttu-id="a4ddc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4ddc-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ddc-121">Request body</span></span>
<span data-ttu-id="a4ddc-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4ddc-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4ddc-123">Parameter</span></span>    | <span data-ttu-id="a4ddc-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4ddc-124">Type</span></span>   |<span data-ttu-id="a4ddc-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4ddc-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4ddc-126">anotherRange</span><span class="sxs-lookup"><span data-stu-id="a4ddc-126">anotherRange</span></span>|<span data-ttu-id="a4ddc-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4ddc-127">string</span></span>|<span data-ttu-id="a4ddc-128">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-128">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="a4ddc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4ddc-129">Response</span></span>

<span data-ttu-id="a4ddc-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ddc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4ddc-131">Example</span></span>
<span data-ttu-id="a4ddc-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4ddc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ddc-133">Request</span></span>
<span data-ttu-id="a4ddc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="a4ddc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4ddc-135">Response</span></span>
<span data-ttu-id="a4ddc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4ddc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
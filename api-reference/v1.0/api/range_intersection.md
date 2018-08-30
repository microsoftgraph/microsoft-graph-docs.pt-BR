# <a name="range-intersection"></a><span data-ttu-id="9d6bb-101">Intervalo: interseção</span><span class="sxs-lookup"><span data-stu-id="9d6bb-101">Range: Intersection</span></span>

<span data-ttu-id="9d6bb-102">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d6bb-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d6bb-103">Permissions</span></span>
<span data-ttu-id="9d6bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d6bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d6bb-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d6bb-106">Permission type</span></span>      | <span data-ttu-id="9d6bb-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d6bb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d6bb-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d6bb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d6bb-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d6bb-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d6bb-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d6bb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d6bb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-111">Not supported.</span></span>    |
|<span data-ttu-id="9d6bb-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d6bb-112">Application</span></span> | <span data-ttu-id="9d6bb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d6bb-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d6bb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="9d6bb-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d6bb-115">Request headers</span></span>
| <span data-ttu-id="9d6bb-116">Nome</span><span class="sxs-lookup"><span data-stu-id="9d6bb-116">Name</span></span>       | <span data-ttu-id="9d6bb-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d6bb-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d6bb-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d6bb-118">Authorization</span></span>  | <span data-ttu-id="9d6bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d6bb-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9d6bb-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9d6bb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6bb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d6bb-124">Request body</span></span>
<span data-ttu-id="9d6bb-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d6bb-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9d6bb-126">Parameter</span></span>    | <span data-ttu-id="9d6bb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d6bb-127">Type</span></span>   |<span data-ttu-id="9d6bb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d6bb-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d6bb-129">anotherRange</span><span class="sxs-lookup"><span data-stu-id="9d6bb-129">anotherRange</span></span>|<span data-ttu-id="9d6bb-130">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d6bb-130">string</span></span>|<span data-ttu-id="9d6bb-131">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-131">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="9d6bb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d6bb-132">Response</span></span>

<span data-ttu-id="9d6bb-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-133">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d6bb-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d6bb-134">Example</span></span>
<span data-ttu-id="9d6bb-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9d6bb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d6bb-136">Request</span></span>
<span data-ttu-id="9d6bb-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="9d6bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d6bb-138">Response</span></span>
<span data-ttu-id="9d6bb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
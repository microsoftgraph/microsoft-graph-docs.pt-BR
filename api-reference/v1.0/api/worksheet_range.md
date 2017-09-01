# <a name="worksheet-range"></a><span data-ttu-id="5acc0-101">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="5acc0-101">Worksheet: Range</span></span>

<span data-ttu-id="5acc0-102">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="5acc0-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="5acc0-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5acc0-103">Permissions</span></span>
<span data-ttu-id="5acc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5acc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5acc0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5acc0-106">Permission type</span></span>      | <span data-ttu-id="5acc0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5acc0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5acc0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5acc0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5acc0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5acc0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5acc0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5acc0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5acc0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5acc0-111">Not supported.</span></span>    |
|<span data-ttu-id="5acc0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5acc0-112">Application</span></span> | <span data-ttu-id="5acc0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5acc0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5acc0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5acc0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="5acc0-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5acc0-115">Request headers</span></span>
| <span data-ttu-id="5acc0-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5acc0-116">Name</span></span>       | <span data-ttu-id="5acc0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5acc0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5acc0-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="5acc0-118">Authorization</span></span>  | <span data-ttu-id="5acc0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5acc0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5acc0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5acc0-121">Request body</span></span>
<span data-ttu-id="5acc0-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5acc0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5acc0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5acc0-123">Parameter</span></span>    | <span data-ttu-id="5acc0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5acc0-124">Type</span></span>   |<span data-ttu-id="5acc0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5acc0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5acc0-126">address</span><span class="sxs-lookup"><span data-stu-id="5acc0-126">address</span></span>|<span data-ttu-id="5acc0-127">string</span><span class="sxs-lookup"><span data-stu-id="5acc0-127">string</span></span>|<span data-ttu-id="5acc0-p103">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="5acc0-p103">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="5acc0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5acc0-131">Response</span></span>

<span data-ttu-id="5acc0-132">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5acc0-132">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5acc0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5acc0-133">Example</span></span>
<span data-ttu-id="5acc0-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5acc0-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5acc0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5acc0-135">Request</span></span>
<span data-ttu-id="5acc0-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5acc0-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="5acc0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5acc0-137">Response</span></span>
<span data-ttu-id="5acc0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5acc0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
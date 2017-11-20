# <a name="rangebordercollection-itemat"></a><span data-ttu-id="42bdc-101">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="42bdc-101">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="42bdc-102">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="42bdc-102">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="42bdc-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="42bdc-103">Permissions</span></span>
<span data-ttu-id="42bdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="42bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="42bdc-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42bdc-106">Permission type</span></span>      | <span data-ttu-id="42bdc-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42bdc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42bdc-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42bdc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="42bdc-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42bdc-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42bdc-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42bdc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42bdc-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42bdc-111">Not supported.</span></span>    |
|<span data-ttu-id="42bdc-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42bdc-112">Application</span></span> | <span data-ttu-id="42bdc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42bdc-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42bdc-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42bdc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="42bdc-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42bdc-115">Request headers</span></span>
| <span data-ttu-id="42bdc-116">Nome</span><span class="sxs-lookup"><span data-stu-id="42bdc-116">Name</span></span>       | <span data-ttu-id="42bdc-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="42bdc-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42bdc-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="42bdc-118">Authorization</span></span>  | <span data-ttu-id="42bdc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42bdc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42bdc-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42bdc-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="42bdc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="42bdc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42bdc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42bdc-124">Request body</span></span>
<span data-ttu-id="42bdc-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42bdc-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42bdc-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="42bdc-126">Parameter</span></span>    | <span data-ttu-id="42bdc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="42bdc-127">Type</span></span>   |<span data-ttu-id="42bdc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="42bdc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42bdc-129">index</span><span class="sxs-lookup"><span data-stu-id="42bdc-129">index</span></span>|<span data-ttu-id="42bdc-130">number</span><span class="sxs-lookup"><span data-stu-id="42bdc-130">number</span></span>|<span data-ttu-id="42bdc-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="42bdc-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="42bdc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="42bdc-133">Response</span></span>

<span data-ttu-id="42bdc-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [RangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42bdc-134">If successful, this method returns `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42bdc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42bdc-135">Example</span></span>
<span data-ttu-id="42bdc-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="42bdc-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="42bdc-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42bdc-137">Request</span></span>
<span data-ttu-id="42bdc-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42bdc-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="42bdc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42bdc-139">Response</span></span>
<span data-ttu-id="42bdc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42bdc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
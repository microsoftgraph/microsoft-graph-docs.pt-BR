# <a name="create-rangeborder"></a><span data-ttu-id="2fb6d-101">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2fb6d-101">Create RangeBorder</span></span>

<span data-ttu-id="2fb6d-102">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fb6d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fb6d-103">Permissions</span></span>
<span data-ttu-id="2fb6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2fb6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2fb6d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fb6d-106">Permission type</span></span>      | <span data-ttu-id="2fb6d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fb6d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fb6d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fb6d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2fb6d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fb6d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fb6d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fb6d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fb6d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-111">Not supported.</span></span>    |
|<span data-ttu-id="2fb6d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fb6d-112">Application</span></span> | <span data-ttu-id="2fb6d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fb6d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fb6d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="2fb6d-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb6d-115">Request headers</span></span>
| <span data-ttu-id="2fb6d-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2fb6d-116">Name</span></span>       | <span data-ttu-id="2fb6d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fb6d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fb6d-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fb6d-118">Authorization</span></span>  | <span data-ttu-id="2fb6d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fb6d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2fb6d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2fb6d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb6d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb6d-124">Request body</span></span>
<span data-ttu-id="2fb6d-125">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookRangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="2fb6d-125">In the request body, supply a JSON representation of [directoryObject](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2fb6d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fb6d-126">Response</span></span>

<span data-ttu-id="2fb6d-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb6d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fb6d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fb6d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb6d-129">Request</span></span>
<span data-ttu-id="2fb6d-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
<span data-ttu-id="2fb6d-131">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookRangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="2fb6d-131">In the request body, supply a JSON representation of [plannerPlan](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2fb6d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fb6d-132">Response</span></span>
<span data-ttu-id="2fb6d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fb6d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
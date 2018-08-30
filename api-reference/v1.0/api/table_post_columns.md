# <a name="create-tablecolumn"></a><span data-ttu-id="eb6be-101">Criar TableColumn</span><span class="sxs-lookup"><span data-stu-id="eb6be-101">Create TableColumn</span></span>

<span data-ttu-id="eb6be-102">Use essa API para criar uma nova TableColumn.</span><span class="sxs-lookup"><span data-stu-id="eb6be-102">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb6be-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb6be-103">Permissions</span></span>
<span data-ttu-id="eb6be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb6be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb6be-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb6be-106">Permission type</span></span>      | <span data-ttu-id="eb6be-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb6be-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb6be-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb6be-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eb6be-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb6be-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb6be-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb6be-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb6be-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6be-111">Not supported.</span></span>    |
|<span data-ttu-id="eb6be-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb6be-112">Application</span></span> | <span data-ttu-id="eb6be-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6be-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb6be-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6be-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="eb6be-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6be-115">Request headers</span></span>
| <span data-ttu-id="eb6be-116">Nome</span><span class="sxs-lookup"><span data-stu-id="eb6be-116">Name</span></span>       | <span data-ttu-id="eb6be-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb6be-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb6be-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb6be-118">Authorization</span></span>  | <span data-ttu-id="eb6be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb6be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb6be-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eb6be-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="eb6be-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb6be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb6be-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6be-124">Request body</span></span>
<span data-ttu-id="eb6be-125">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookTableColumn](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="eb6be-125">In the request body, supply a JSON representation of [directoryObject](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eb6be-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6be-126">Response</span></span>

<span data-ttu-id="eb6be-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [WorkbookTableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb6be-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb6be-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb6be-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb6be-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6be-129">Request</span></span>
<span data-ttu-id="eb6be-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb6be-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="eb6be-131">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookTableColumn](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="eb6be-131">In the request body, supply a JSON representation of [plannerPlan](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eb6be-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6be-132">Response</span></span>
<span data-ttu-id="eb6be-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb6be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
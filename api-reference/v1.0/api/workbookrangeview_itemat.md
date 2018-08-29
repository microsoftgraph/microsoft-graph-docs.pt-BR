# <a name="workbookrangeview-itemat"></a><span data-ttu-id="3d37a-101">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="3d37a-101">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="3d37a-102">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d37a-102">Permissions</span></span>
<span data-ttu-id="3d37a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d37a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d37a-105">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d37a-105">Permission type</span></span>      | <span data-ttu-id="3d37a-106">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d37a-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d37a-107">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d37a-107">Delegated (work or school account)</span></span> | <span data-ttu-id="3d37a-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d37a-108">Files.ReadWrite</span></span> |
|<span data-ttu-id="3d37a-109">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d37a-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d37a-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d37a-110">Not supported.</span></span>    |
|<span data-ttu-id="3d37a-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d37a-111">Application</span></span> | <span data-ttu-id="3d37a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d37a-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d37a-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d37a-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="3d37a-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d37a-114">Request headers</span></span>
| <span data-ttu-id="3d37a-115">Nome</span><span class="sxs-lookup"><span data-stu-id="3d37a-115">Name</span></span>       | <span data-ttu-id="3d37a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d37a-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d37a-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d37a-117">Authorization</span></span>  | <span data-ttu-id="3d37a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d37a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d37a-120">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d37a-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d37a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d37a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="3d37a-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3d37a-123">Function parameters</span></span>
<span data-ttu-id="3d37a-124">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="3d37a-124">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="3d37a-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3d37a-125">Parameter</span></span>    | <span data-ttu-id="3d37a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d37a-126">Type</span></span>   |<span data-ttu-id="3d37a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d37a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d37a-128">índice</span><span class="sxs-lookup"><span data-stu-id="3d37a-128">index</span></span>|<span data-ttu-id="3d37a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="3d37a-129">Int32</span></span>|<span data-ttu-id="3d37a-130">O índice do item a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="3d37a-130">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="3d37a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d37a-131">Response</span></span>

<span data-ttu-id="3d37a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d37a-132">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d37a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d37a-133">Example</span></span>
<span data-ttu-id="3d37a-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3d37a-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3d37a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d37a-135">Request</span></span>
<span data-ttu-id="3d37a-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d37a-136">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="3d37a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d37a-137">Response</span></span>
<span data-ttu-id="3d37a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d37a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```

# <a name="workbookrange-visibleview"></a><span data-ttu-id="ec588-101">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="ec588-101">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="ec588-102">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec588-102">Permissions</span></span>
<span data-ttu-id="ec588-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec588-105">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec588-105">Permission type</span></span>      | <span data-ttu-id="ec588-106">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec588-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec588-107">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec588-107">Delegated (work or school account)</span></span> | <span data-ttu-id="ec588-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec588-108">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec588-109">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec588-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec588-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec588-110">Not supported.</span></span>    |
|<span data-ttu-id="ec588-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec588-111">Application</span></span> | <span data-ttu-id="ec588-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec588-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec588-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec588-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="ec588-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec588-114">Request headers</span></span>
| <span data-ttu-id="ec588-115">Nome</span><span class="sxs-lookup"><span data-stu-id="ec588-115">Name</span></span>       | <span data-ttu-id="ec588-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec588-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec588-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec588-117">Authorization</span></span>  | <span data-ttu-id="ec588-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec588-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec588-120">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec588-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec588-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ec588-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec588-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec588-123">Request body</span></span>

### <a name="response"></a><span data-ttu-id="ec588-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec588-124">Response</span></span>
<span data-ttu-id="ec588-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec588-125">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec588-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec588-126">Example</span></span>
<span data-ttu-id="ec588-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ec588-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec588-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec588-128">Request</span></span>
<span data-ttu-id="ec588-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec588-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="ec588-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec588-130">Response</span></span>
<span data-ttu-id="ec588-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec588-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
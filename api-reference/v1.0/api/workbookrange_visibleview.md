# <a name="workbookrange-visibleview"></a><span data-ttu-id="54e0f-101">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="54e0f-101">workbookRange: visibleView</span></span>


## <a name="prerequisites"></a><span data-ttu-id="54e0f-102">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54e0f-102">Prerequisites</span></span>
<span data-ttu-id="54e0f-103">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="54e0f-103">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="54e0f-104">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54e0f-104">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="54e0f-105">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54e0f-105">Request headers</span></span>
| <span data-ttu-id="54e0f-106">Nome</span><span class="sxs-lookup"><span data-stu-id="54e0f-106">Name</span></span>       | <span data-ttu-id="54e0f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e0f-107">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="54e0f-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="54e0f-108">Authorization</span></span>  | <span data-ttu-id="54e0f-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54e0f-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54e0f-111">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="54e0f-111">Workbook-Session-Id</span></span>  | <span data-ttu-id="54e0f-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="54e0f-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54e0f-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54e0f-114">Request body</span></span>

## <a name="response"></a><span data-ttu-id="54e0f-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="54e0f-115">Response</span></span>

<span data-ttu-id="54e0f-116">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54e0f-116">If successful, this method returns `200, OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54e0f-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54e0f-117">Example</span></span>
<span data-ttu-id="54e0f-118">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="54e0f-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="54e0f-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54e0f-119">Request</span></span>
<span data-ttu-id="54e0f-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54e0f-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="54e0f-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="54e0f-121">Response</span></span>
<span data-ttu-id="54e0f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54e0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
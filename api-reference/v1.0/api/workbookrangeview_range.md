# <a name="workbookrangeview-range"></a><span data-ttu-id="bb5b0-101">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="bb5b0-101">workbookRangeView: range</span></span>
<span data-ttu-id="bb5b0-102">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-102">Return the range associated with the rangeView resource.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb5b0-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb5b0-103">Prerequisites</span></span>
<span data-ttu-id="bb5b0-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="bb5b0-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>

## <a name="http-request"></a><span data-ttu-id="bb5b0-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb5b0-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="bb5b0-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5b0-106">Request headers</span></span>
| <span data-ttu-id="bb5b0-107">Nome</span><span class="sxs-lookup"><span data-stu-id="bb5b0-107">Name</span></span>       | <span data-ttu-id="bb5b0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb5b0-108">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb5b0-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb5b0-109">Authorization</span></span>  | <span data-ttu-id="bb5b0-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb5b0-112">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bb5b0-112">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb5b0-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb5b0-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5b0-115">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bb5b0-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5b0-116">Response</span></span>

<span data-ttu-id="bb5b0-117">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-117">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb5b0-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb5b0-118">Example</span></span>
<span data-ttu-id="bb5b0-119">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb5b0-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5b0-120">Request</span></span>
<span data-ttu-id="bb5b0-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="bb5b0-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5b0-122">Response</span></span>
<span data-ttu-id="bb5b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

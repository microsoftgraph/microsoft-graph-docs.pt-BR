# <a name="workbookrangeview-range"></a><span data-ttu-id="b3599-101">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="b3599-101">workbookRangeView: range</span></span>
<span data-ttu-id="b3599-102">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="b3599-102">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3599-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3599-103">Permissions</span></span>
<span data-ttu-id="b3599-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b3599-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3599-106">Permission type</span></span>      | <span data-ttu-id="b3599-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3599-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3599-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3599-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b3599-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3599-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b3599-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3599-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3599-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3599-111">Not supported.</span></span>    |
|<span data-ttu-id="b3599-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3599-112">Application</span></span> | <span data-ttu-id="b3599-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3599-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3599-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3599-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="b3599-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3599-115">Request headers</span></span>
| <span data-ttu-id="b3599-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b3599-116">Name</span></span>       | <span data-ttu-id="b3599-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3599-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3599-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3599-118">Authorization</span></span>  | <span data-ttu-id="b3599-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3599-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3599-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b3599-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b3599-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b3599-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3599-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3599-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="b3599-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3599-125">Response</span></span>
<span data-ttu-id="b3599-126">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3599-126">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3599-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3599-127">Example</span></span>
<span data-ttu-id="b3599-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b3599-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b3599-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3599-129">Request</span></span>
<span data-ttu-id="b3599-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3599-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="b3599-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3599-131">Response</span></span>
<span data-ttu-id="b3599-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3599-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

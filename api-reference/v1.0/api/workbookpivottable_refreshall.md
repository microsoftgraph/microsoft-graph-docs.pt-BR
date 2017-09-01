# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="76161-101">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="76161-101">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="76161-102">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="76161-102">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="76161-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="76161-103">Permissions</span></span>
<span data-ttu-id="76161-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76161-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76161-106">Permission type</span></span>      | <span data-ttu-id="76161-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76161-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76161-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76161-108">Delegated (work or school account)</span></span> | <span data-ttu-id="76161-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76161-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="76161-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76161-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76161-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76161-111">Not supported.</span></span>    |
|<span data-ttu-id="76161-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76161-112">Application</span></span> | <span data-ttu-id="76161-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76161-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76161-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76161-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="76161-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76161-115">Request headers</span></span>
| <span data-ttu-id="76161-116">Nome</span><span class="sxs-lookup"><span data-stu-id="76161-116">Name</span></span>       | <span data-ttu-id="76161-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="76161-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76161-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="76161-118">Authorization</span></span>  | <span data-ttu-id="76161-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76161-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76161-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76161-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="76161-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="76161-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76161-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76161-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="76161-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="76161-125">Response</span></span>
<span data-ttu-id="76161-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76161-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76161-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76161-128">Example</span></span>
<span data-ttu-id="76161-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="76161-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76161-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76161-130">Request</span></span>
<span data-ttu-id="76161-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76161-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="76161-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="76161-132">Response</span></span>
<span data-ttu-id="76161-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76161-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

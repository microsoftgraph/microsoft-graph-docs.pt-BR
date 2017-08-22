# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="fa39c-101">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="fa39c-101">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="fa39c-102">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="fa39c-102">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa39c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa39c-103">Prerequisites</span></span>
<span data-ttu-id="fa39c-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="fa39c-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="fa39c-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa39c-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="fa39c-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa39c-106">Request headers</span></span>
| <span data-ttu-id="fa39c-107">Nome</span><span class="sxs-lookup"><span data-stu-id="fa39c-107">Name</span></span>       | <span data-ttu-id="fa39c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa39c-108">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa39c-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa39c-109">Authorization</span></span>  | <span data-ttu-id="fa39c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa39c-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa39c-112">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fa39c-112">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa39c-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fa39c-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa39c-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa39c-115">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fa39c-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa39c-116">Response</span></span>

<span data-ttu-id="fa39c-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa39c-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa39c-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa39c-119">Example</span></span>
<span data-ttu-id="fa39c-120">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fa39c-120">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa39c-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa39c-121">Request</span></span>
<span data-ttu-id="fa39c-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa39c-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="fa39c-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa39c-123">Response</span></span>
<span data-ttu-id="fa39c-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa39c-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

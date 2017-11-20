# <a name="chartlineformat-clear"></a><span data-ttu-id="d12b1-101">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="d12b1-101">ChartLineFormat: clear</span></span>

<span data-ttu-id="d12b1-102">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d12b1-102">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="d12b1-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d12b1-103">Permissions</span></span>
<span data-ttu-id="d12b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d12b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d12b1-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d12b1-106">Permission type</span></span>      | <span data-ttu-id="d12b1-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d12b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d12b1-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d12b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d12b1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d12b1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d12b1-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d12b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d12b1-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d12b1-111">Not supported.</span></span>    |
|<span data-ttu-id="d12b1-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d12b1-112">Application</span></span> | <span data-ttu-id="d12b1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d12b1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d12b1-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d12b1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="d12b1-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d12b1-115">Request headers</span></span>
| <span data-ttu-id="d12b1-116">Nome</span><span class="sxs-lookup"><span data-stu-id="d12b1-116">Name</span></span>       | <span data-ttu-id="d12b1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d12b1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d12b1-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="d12b1-118">Authorization</span></span>  | <span data-ttu-id="d12b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d12b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d12b1-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d12b1-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="d12b1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d12b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d12b1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d12b1-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d12b1-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d12b1-125">Response</span></span>

<span data-ttu-id="d12b1-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d12b1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d12b1-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d12b1-128">Example</span></span>
<span data-ttu-id="d12b1-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d12b1-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d12b1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d12b1-130">Request</span></span>
<span data-ttu-id="d12b1-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d12b1-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="d12b1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d12b1-132">Response</span></span>
<span data-ttu-id="d12b1-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d12b1-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
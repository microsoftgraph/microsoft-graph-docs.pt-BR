# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="980dd-101">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="980dd-101">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="980dd-102">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="980dd-102">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="980dd-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="980dd-103">Permissions</span></span>
<span data-ttu-id="980dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="980dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="980dd-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="980dd-106">Permission type</span></span>      | <span data-ttu-id="980dd-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="980dd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="980dd-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="980dd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="980dd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="980dd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="980dd-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="980dd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="980dd-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="980dd-111">Not supported.</span></span>    |
|<span data-ttu-id="980dd-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="980dd-112">Application</span></span> | <span data-ttu-id="980dd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="980dd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="980dd-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="980dd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="980dd-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="980dd-115">Request headers</span></span>
| <span data-ttu-id="980dd-116">Nome</span><span class="sxs-lookup"><span data-stu-id="980dd-116">Name</span></span>       | <span data-ttu-id="980dd-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="980dd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="980dd-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="980dd-118">Authorization</span></span>  | <span data-ttu-id="980dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="980dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="980dd-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="980dd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="980dd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="980dd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="980dd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="980dd-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="980dd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="980dd-125">Response</span></span>

<span data-ttu-id="980dd-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="980dd-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="980dd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="980dd-128">Example</span></span>
<span data-ttu-id="980dd-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="980dd-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="980dd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="980dd-130">Request</span></span>
<span data-ttu-id="980dd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="980dd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="980dd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="980dd-132">Response</span></span>
<span data-ttu-id="980dd-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="980dd-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
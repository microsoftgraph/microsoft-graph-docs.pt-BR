# <a name="filter-clear"></a><span data-ttu-id="67241-101">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="67241-101">Filter: clear</span></span>

<span data-ttu-id="67241-102">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="67241-102">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="67241-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="67241-103">Permissions</span></span>
<span data-ttu-id="67241-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="67241-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="67241-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67241-106">Permission type</span></span>      | <span data-ttu-id="67241-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67241-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67241-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67241-108">Delegated (work or school account)</span></span> | <span data-ttu-id="67241-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67241-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67241-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67241-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67241-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67241-111">Not supported.</span></span>    |
|<span data-ttu-id="67241-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67241-112">Application</span></span> | <span data-ttu-id="67241-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67241-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67241-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67241-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="67241-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67241-115">Request headers</span></span>
| <span data-ttu-id="67241-116">Nome</span><span class="sxs-lookup"><span data-stu-id="67241-116">Name</span></span>       | <span data-ttu-id="67241-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="67241-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67241-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="67241-118">Authorization</span></span>  | <span data-ttu-id="67241-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67241-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67241-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67241-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="67241-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="67241-122">Response</span></span>

<span data-ttu-id="67241-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67241-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67241-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67241-125">Example</span></span>
<span data-ttu-id="67241-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="67241-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67241-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67241-127">Request</span></span>
<span data-ttu-id="67241-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67241-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="67241-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67241-129">Response</span></span>
<span data-ttu-id="67241-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67241-130">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
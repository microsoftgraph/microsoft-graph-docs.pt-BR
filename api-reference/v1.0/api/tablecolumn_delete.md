# <a name="tablecolumn-delete"></a><span data-ttu-id="c500b-101">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="c500b-101">TableColumn: delete</span></span>

<span data-ttu-id="c500b-102">Exclui a coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="c500b-102">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c500b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c500b-103">Permissions</span></span>
<span data-ttu-id="c500b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c500b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c500b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c500b-106">Permission type</span></span>      | <span data-ttu-id="c500b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c500b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c500b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c500b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c500b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c500b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c500b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c500b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c500b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c500b-111">Not supported.</span></span>    |
|<span data-ttu-id="c500b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c500b-112">Application</span></span> | <span data-ttu-id="c500b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c500b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c500b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c500b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="c500b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c500b-115">Request headers</span></span>
| <span data-ttu-id="c500b-116">Nome</span><span class="sxs-lookup"><span data-stu-id="c500b-116">Name</span></span>       | <span data-ttu-id="c500b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c500b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c500b-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="c500b-118">Authorization</span></span>  | <span data-ttu-id="c500b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c500b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c500b-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c500b-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c500b-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="c500b-122">Response</span></span>

<span data-ttu-id="c500b-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c500b-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c500b-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c500b-125">Example</span></span>
<span data-ttu-id="c500b-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c500b-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c500b-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c500b-127">Request</span></span>
<span data-ttu-id="c500b-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c500b-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="c500b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c500b-129">Response</span></span>
<span data-ttu-id="c500b-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c500b-130">Here is an example of the response.</span></span> 
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
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
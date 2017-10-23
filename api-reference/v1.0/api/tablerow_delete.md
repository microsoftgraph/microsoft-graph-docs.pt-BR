# <a name="tablerow-delete"></a><span data-ttu-id="67472-101">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="67472-101">TableRow: delete</span></span>

<span data-ttu-id="67472-102">Exclui a linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="67472-102">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="67472-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="67472-103">Permissions</span></span>
<span data-ttu-id="67472-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="67472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="67472-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67472-106">Permission type</span></span>      | <span data-ttu-id="67472-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67472-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67472-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67472-108">Delegated (work or school account)</span></span> | <span data-ttu-id="67472-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67472-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67472-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67472-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67472-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67472-111">Not supported.</span></span>    |
|<span data-ttu-id="67472-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67472-112">Application</span></span> | <span data-ttu-id="67472-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67472-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67472-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67472-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="67472-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67472-115">Request headers</span></span>
| <span data-ttu-id="67472-116">Nome</span><span class="sxs-lookup"><span data-stu-id="67472-116">Name</span></span>       | <span data-ttu-id="67472-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="67472-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67472-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="67472-118">Authorization</span></span>  | <span data-ttu-id="67472-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67472-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67472-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67472-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="67472-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="67472-122">Response</span></span>

<span data-ttu-id="67472-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67472-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67472-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67472-125">Example</span></span>
<span data-ttu-id="67472-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="67472-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67472-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67472-127">Request</span></span>
<span data-ttu-id="67472-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67472-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="67472-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67472-129">Response</span></span>
<span data-ttu-id="67472-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67472-130">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
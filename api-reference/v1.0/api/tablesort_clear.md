# <a name="tablesort-clear"></a><span data-ttu-id="e2640-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="e2640-101">TableSort: clear</span></span>

<span data-ttu-id="e2640-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e2640-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2640-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2640-104">Permissions</span></span>
<span data-ttu-id="e2640-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2640-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e2640-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2640-107">Permission type</span></span>      | <span data-ttu-id="e2640-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2640-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2640-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2640-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e2640-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2640-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2640-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2640-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2640-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2640-112">Not supported.</span></span>    |
|<span data-ttu-id="e2640-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2640-113">Application</span></span> | <span data-ttu-id="e2640-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2640-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2640-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2640-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="e2640-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2640-116">Request headers</span></span>
| <span data-ttu-id="e2640-117">Nome</span><span class="sxs-lookup"><span data-stu-id="e2640-117">Name</span></span>       | <span data-ttu-id="e2640-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2640-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2640-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2640-119">Authorization</span></span>  | <span data-ttu-id="e2640-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2640-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2640-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2640-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e2640-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2640-123">Response</span></span>

<span data-ttu-id="e2640-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2640-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2640-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2640-126">Example</span></span>
<span data-ttu-id="e2640-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e2640-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2640-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2640-128">Request</span></span>
<span data-ttu-id="e2640-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2640-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="e2640-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2640-130">Response</span></span>
<span data-ttu-id="e2640-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2640-131">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
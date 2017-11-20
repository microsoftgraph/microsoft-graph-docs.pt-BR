# <a name="tablesort-clear"></a><span data-ttu-id="d4918-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="d4918-101">TableSort: clear</span></span>

<span data-ttu-id="d4918-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="d4918-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="d4918-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4918-104">Permissions</span></span>
<span data-ttu-id="d4918-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4918-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d4918-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4918-107">Permission type</span></span>      | <span data-ttu-id="d4918-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4918-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4918-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4918-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d4918-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4918-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d4918-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4918-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4918-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4918-112">Not supported.</span></span>    |
|<span data-ttu-id="d4918-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4918-113">Application</span></span> | <span data-ttu-id="d4918-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4918-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4918-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4918-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="d4918-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4918-116">Request headers</span></span>
| <span data-ttu-id="d4918-117">Nome</span><span class="sxs-lookup"><span data-stu-id="d4918-117">Name</span></span>       | <span data-ttu-id="d4918-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4918-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d4918-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4918-119">Authorization</span></span>  | <span data-ttu-id="d4918-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4918-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4918-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d4918-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="d4918-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d4918-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4918-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4918-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d4918-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4918-126">Response</span></span>

<span data-ttu-id="d4918-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4918-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4918-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4918-129">Example</span></span>
<span data-ttu-id="d4918-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d4918-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4918-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4918-131">Request</span></span>
<span data-ttu-id="d4918-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4918-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="d4918-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4918-133">Response</span></span>
<span data-ttu-id="d4918-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4918-134">Here is an example of the response.</span></span> 
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
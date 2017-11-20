# <a name="tablesort-reapply"></a><span data-ttu-id="7c455-101">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="7c455-101">TableSort: reapply</span></span>

<span data-ttu-id="7c455-102">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="7c455-102">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c455-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c455-103">Permissions</span></span>
<span data-ttu-id="7c455-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c455-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c455-106">Permission type</span></span>      | <span data-ttu-id="7c455-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c455-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c455-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c455-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7c455-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c455-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c455-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c455-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c455-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c455-111">Not supported.</span></span>    |
|<span data-ttu-id="7c455-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c455-112">Application</span></span> | <span data-ttu-id="7c455-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c455-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c455-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c455-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="7c455-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c455-115">Request headers</span></span>
| <span data-ttu-id="7c455-116">Nome</span><span class="sxs-lookup"><span data-stu-id="7c455-116">Name</span></span>       | <span data-ttu-id="7c455-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c455-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c455-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c455-118">Authorization</span></span>  | <span data-ttu-id="7c455-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c455-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c455-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c455-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c455-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7c455-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c455-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c455-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7c455-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c455-125">Response</span></span>

<span data-ttu-id="7c455-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c455-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c455-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c455-128">Example</span></span>
<span data-ttu-id="7c455-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7c455-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c455-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c455-130">Request</span></span>
<span data-ttu-id="7c455-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c455-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```

##### <a name="response"></a><span data-ttu-id="7c455-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c455-132">Response</span></span>
<span data-ttu-id="7c455-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c455-133">Here is an example of the response.</span></span> 
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
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
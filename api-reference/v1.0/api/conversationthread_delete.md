# <a name="delete-conversationthread"></a><span data-ttu-id="ea7cb-101">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="ea7cb-101">Delete conversationThread</span></span>

<span data-ttu-id="ea7cb-102">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-102">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea7cb-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea7cb-103">Permissions</span></span>
<span data-ttu-id="ea7cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea7cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea7cb-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea7cb-106">Permission type</span></span>      | <span data-ttu-id="ea7cb-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea7cb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea7cb-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea7cb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ea7cb-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7cb-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea7cb-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea7cb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea7cb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-111">Not supported.</span></span>    |
|<span data-ttu-id="ea7cb-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea7cb-112">Application</span></span> | <span data-ttu-id="ea7cb-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7cb-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea7cb-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea7cb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ea7cb-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea7cb-115">Request headers</span></span>
| <span data-ttu-id="ea7cb-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea7cb-116">Header</span></span>       | <span data-ttu-id="ea7cb-117">Valor</span><span class="sxs-lookup"><span data-stu-id="ea7cb-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea7cb-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea7cb-118">Authorization</span></span>  | <span data-ttu-id="ea7cb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea7cb-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea7cb-121">Request body</span></span>
<span data-ttu-id="ea7cb-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea7cb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea7cb-123">Response</span></span>

<span data-ttu-id="ea7cb-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea7cb-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea7cb-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea7cb-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea7cb-127">Request</span></span>
<span data-ttu-id="ea7cb-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="ea7cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea7cb-129">Response</span></span>
<span data-ttu-id="ea7cb-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea7cb-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
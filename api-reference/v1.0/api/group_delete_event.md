# <a name="delete-event"></a><span data-ttu-id="d9c3e-101">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="d9c3e-101">Delete event</span></span>
<span data-ttu-id="d9c3e-102">Excluir um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d9c3e-102">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9c3e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9c3e-103">Permissions</span></span>
<span data-ttu-id="d9c3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d9c3e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9c3e-106">Permission type</span></span>      | <span data-ttu-id="d9c3e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9c3e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9c3e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9c3e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d9c3e-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c3e-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9c3e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9c3e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9c3e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-111">Not supported.</span></span>    |
|<span data-ttu-id="d9c3e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9c3e-112">Application</span></span> | <span data-ttu-id="d9c3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9c3e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c3e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d9c3e-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c3e-115">Request headers</span></span>
| <span data-ttu-id="d9c3e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="d9c3e-116">Name</span></span>       | <span data-ttu-id="d9c3e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9c3e-117">Type</span></span> | <span data-ttu-id="d9c3e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9c3e-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9c3e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9c3e-119">Authorization</span></span>  | <span data-ttu-id="d9c3e-120">string</span><span class="sxs-lookup"><span data-stu-id="d9c3e-120">string</span></span>  | <span data-ttu-id="d9c3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9c3e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c3e-123">Request body</span></span>
<span data-ttu-id="d9c3e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9c3e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c3e-125">Response</span></span>
<span data-ttu-id="d9c3e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9c3e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9c3e-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d9c3e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c3e-129">Request</span></span>
<span data-ttu-id="d9c3e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-130">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="d9c3e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c3e-131">Response</span></span>
<span data-ttu-id="d9c3e-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-132">Here is an example of the response.</span></span> 
><span data-ttu-id="d9c3e-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d9c3e-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9c3e-134">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
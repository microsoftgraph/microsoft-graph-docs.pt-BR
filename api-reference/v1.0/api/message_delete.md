# <a name="delete-message"></a><span data-ttu-id="da576-101">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="da576-101">Delete message</span></span>

<span data-ttu-id="da576-102">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da576-102">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="da576-103">**Observação** Você não poderá excluir itens da pasta de itens excluídos recuperáveis (representado pelo [nome da pasta conhecido](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="da576-103">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="da576-104">Confira [Retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpeza de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="da576-104">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="da576-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da576-105">Permissions</span></span>
<span data-ttu-id="da576-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da576-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da576-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da576-108">Permission type</span></span>      | <span data-ttu-id="da576-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da576-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da576-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da576-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da576-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da576-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da576-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da576-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da576-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da576-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da576-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da576-114">Application</span></span> | <span data-ttu-id="da576-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da576-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da576-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da576-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da576-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da576-117">Request headers</span></span>
| <span data-ttu-id="da576-118">Nome</span><span class="sxs-lookup"><span data-stu-id="da576-118">Name</span></span>       | <span data-ttu-id="da576-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="da576-119">Type</span></span> | <span data-ttu-id="da576-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da576-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da576-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da576-121">Authorization</span></span>  | <span data-ttu-id="da576-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="da576-122">string</span></span>  | <span data-ttu-id="da576-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da576-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da576-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da576-125">Request body</span></span>
<span data-ttu-id="da576-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da576-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da576-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="da576-127">Response</span></span>

<span data-ttu-id="da576-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da576-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da576-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da576-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da576-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da576-131">Request</span></span>
<span data-ttu-id="da576-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da576-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="da576-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="da576-133">Response</span></span>
<span data-ttu-id="da576-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da576-134">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
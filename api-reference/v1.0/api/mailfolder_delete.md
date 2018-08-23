# <a name="delete-mailfolder"></a><span data-ttu-id="3d199-101">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="3d199-101">Delete mailFolder</span></span>

<span data-ttu-id="3d199-102">Excluir o objeto [mailFolder](../resources/mailfolder.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="3d199-102">Delete the specified mailFolder object.</span></span>

<span data-ttu-id="3d199-103">Você pode especificar uma pasta de email por sua ID de pasta, ou por seu [nome da pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="3d199-103">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="3d199-104">**Observação** Você não poderá excluir itens na pasta de itens excluídos recuperáveis (representado pelo nome da pasta conhecido `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="3d199-104">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="3d199-105">Confira [Retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpeza de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="3d199-105">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d199-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d199-106">Permissions</span></span>
<span data-ttu-id="3d199-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d199-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d199-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d199-109">Permission type</span></span>      | <span data-ttu-id="3d199-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d199-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d199-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d199-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d199-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d199-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3d199-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d199-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d199-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d199-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3d199-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d199-115">Application</span></span> | <span data-ttu-id="3d199-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d199-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d199-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d199-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3d199-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d199-118">Request headers</span></span>
| <span data-ttu-id="3d199-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3d199-119">Name</span></span>       | <span data-ttu-id="3d199-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d199-120">Type</span></span> | <span data-ttu-id="3d199-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d199-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3d199-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d199-122">Authorization</span></span>  | <span data-ttu-id="3d199-123">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d199-123">string</span></span>  | <span data-ttu-id="3d199-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d199-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d199-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d199-126">Request body</span></span>
<span data-ttu-id="3d199-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d199-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d199-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d199-128">Response</span></span>

<span data-ttu-id="3d199-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d199-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d199-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d199-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d199-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d199-132">Request</span></span>
<span data-ttu-id="3d199-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d199-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="3d199-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d199-134">Response</span></span>
<span data-ttu-id="3d199-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d199-135">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
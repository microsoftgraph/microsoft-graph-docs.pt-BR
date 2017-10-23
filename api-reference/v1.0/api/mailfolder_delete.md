# <a name="delete-mailfolder"></a><span data-ttu-id="a5daa-101">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="a5daa-101">Delete mailFolder</span></span>

<span data-ttu-id="a5daa-102">Exclua a mailFolder.</span><span class="sxs-lookup"><span data-stu-id="a5daa-102">Delete mailFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5daa-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5daa-103">Permissions</span></span>
<span data-ttu-id="a5daa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5daa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5daa-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5daa-106">Permission type</span></span>      | <span data-ttu-id="a5daa-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5daa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5daa-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5daa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a5daa-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5daa-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a5daa-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5daa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5daa-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5daa-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a5daa-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5daa-112">Application</span></span> | <span data-ttu-id="a5daa-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5daa-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5daa-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5daa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a5daa-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5daa-115">Request headers</span></span>
| <span data-ttu-id="a5daa-116">Nome</span><span class="sxs-lookup"><span data-stu-id="a5daa-116">Name</span></span>       | <span data-ttu-id="a5daa-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5daa-117">Type</span></span> | <span data-ttu-id="a5daa-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5daa-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5daa-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5daa-119">Authorization</span></span>  | <span data-ttu-id="a5daa-120">string</span><span class="sxs-lookup"><span data-stu-id="a5daa-120">string</span></span>  | <span data-ttu-id="a5daa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5daa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5daa-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5daa-123">Request body</span></span>
<span data-ttu-id="a5daa-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5daa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5daa-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5daa-125">Response</span></span>

<span data-ttu-id="a5daa-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5daa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5daa-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5daa-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5daa-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5daa-129">Request</span></span>
<span data-ttu-id="a5daa-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5daa-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="a5daa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5daa-131">Response</span></span>
<span data-ttu-id="a5daa-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5daa-132">Here is an example of the response.</span></span> 
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
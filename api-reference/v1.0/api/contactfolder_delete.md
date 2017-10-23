# <a name="delete-contactfolder"></a><span data-ttu-id="8ff5a-101">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="8ff5a-101">Delete contactFolder</span></span>

<span data-ttu-id="8ff5a-102">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="8ff5a-102">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ff5a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ff5a-103">Permissions</span></span>
<span data-ttu-id="8ff5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ff5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ff5a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff5a-106">Permission type</span></span>      | <span data-ttu-id="8ff5a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ff5a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff5a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff5a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff5a-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff5a-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8ff5a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff5a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff5a-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff5a-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8ff5a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff5a-112">Application</span></span> | <span data-ttu-id="8ff5a-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff5a-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff5a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff5a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8ff5a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff5a-115">Request headers</span></span>
| <span data-ttu-id="8ff5a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="8ff5a-116">Name</span></span>       | <span data-ttu-id="8ff5a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff5a-117">Type</span></span> | <span data-ttu-id="8ff5a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff5a-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ff5a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff5a-119">Authorization</span></span>  | <span data-ttu-id="8ff5a-120">string</span><span class="sxs-lookup"><span data-stu-id="8ff5a-120">string</span></span>  | <span data-ttu-id="8ff5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff5a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff5a-123">Request body</span></span>
<span data-ttu-id="8ff5a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ff5a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff5a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff5a-125">Response</span></span>

<span data-ttu-id="8ff5a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff5a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff5a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff5a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff5a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff5a-129">Request</span></span>
<span data-ttu-id="8ff5a-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff5a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="8ff5a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff5a-131">Response</span></span>
<span data-ttu-id="8ff5a-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff5a-132">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

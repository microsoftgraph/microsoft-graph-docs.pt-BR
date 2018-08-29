# <a name="delete-messagerule"></a><span data-ttu-id="b31fd-101">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="b31fd-101">Delete messageRule</span></span>


<span data-ttu-id="b31fd-102">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="b31fd-102">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b31fd-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b31fd-103">Permissions</span></span>
<span data-ttu-id="b31fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b31fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b31fd-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b31fd-106">Permission type</span></span>      | <span data-ttu-id="b31fd-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b31fd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b31fd-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b31fd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b31fd-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b31fd-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b31fd-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b31fd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b31fd-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b31fd-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b31fd-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b31fd-112">Application</span></span> | <span data-ttu-id="b31fd-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b31fd-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b31fd-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b31fd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b31fd-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b31fd-115">Request headers</span></span>
| <span data-ttu-id="b31fd-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b31fd-116">Name</span></span>       | <span data-ttu-id="b31fd-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b31fd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b31fd-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="b31fd-118">Authorization</span></span>  | <span data-ttu-id="b31fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b31fd-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b31fd-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b31fd-121">Request body</span></span>
<span data-ttu-id="b31fd-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b31fd-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b31fd-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="b31fd-123">Response</span></span>
<span data-ttu-id="b31fd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b31fd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b31fd-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b31fd-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b31fd-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b31fd-127">Request</span></span>
<span data-ttu-id="b31fd-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b31fd-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="b31fd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b31fd-129">Response</span></span>
<span data-ttu-id="b31fd-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b31fd-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="delete-directoryobject"></a><span data-ttu-id="70277-101">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="70277-101">Delete directoryObject</span></span>

<span data-ttu-id="70277-102">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="70277-102">Deletes a directoryObject.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70277-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70277-103">Prerequisites</span></span>
<span data-ttu-id="70277-104">Os seguintes **scopes** são necessário para executar esta API: _Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="70277-104">The following **scopes** is required to execute this API: _Directory.AccessAsUser.All_</span></span>

<span data-ttu-id="70277-p101">**OBSERVAÇÃO:** usuários, grupos e contatos são tipos de objeto de diretório. Como resultado, se você precisar excluir usuários, o seguinte **scope** pode e deve ser usado: _User.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="70277-p101">**NOTE:** Users, groups, and contacts are types of directory object. As a result,if you need to delete users, the following **scope** can and should be used: _User.ReadWrite.All_</span></span>
## <a name="http-request"></a><span data-ttu-id="70277-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70277-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="70277-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70277-108">Request headers</span></span>
| <span data-ttu-id="70277-109">Nome</span><span class="sxs-lookup"><span data-stu-id="70277-109">Name</span></span>       | <span data-ttu-id="70277-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="70277-110">Type</span></span> | <span data-ttu-id="70277-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="70277-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70277-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="70277-112">Authorization</span></span>  | <span data-ttu-id="70277-113">string</span><span class="sxs-lookup"><span data-stu-id="70277-113">string</span></span>  | <span data-ttu-id="70277-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70277-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70277-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70277-116">Request body</span></span>
<span data-ttu-id="70277-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70277-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70277-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="70277-118">Response</span></span>

<span data-ttu-id="70277-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70277-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70277-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70277-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70277-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70277-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="70277-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="70277-123">Response</span></span>

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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
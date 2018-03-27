# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="65435-101">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="65435-101">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="65435-102">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65435-102">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65435-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="65435-103">Permissions</span></span>

<span data-ttu-id="65435-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65435-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65435-106">Permission type</span></span>      | <span data-ttu-id="65435-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65435-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65435-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65435-108">Delegated (work or school account)</span></span> | <span data-ttu-id="65435-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65435-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="65435-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65435-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65435-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65435-111">Not supported.</span></span>    |
|<span data-ttu-id="65435-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65435-112">Application</span></span> | <span data-ttu-id="65435-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65435-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65435-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65435-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="65435-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65435-115">Request headers</span></span>

| <span data-ttu-id="65435-116">Nome</span><span class="sxs-lookup"><span data-stu-id="65435-116">Name</span></span> | <span data-ttu-id="65435-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="65435-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="65435-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="65435-118">Authorization</span></span> | <span data-ttu-id="65435-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65435-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65435-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65435-121">Content-Type</span></span>  | <span data-ttu-id="65435-122">application/json</span><span class="sxs-lookup"><span data-stu-id="65435-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="65435-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65435-123">Request body</span></span>
<span data-ttu-id="65435-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65435-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="65435-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="65435-125">Response</span></span>

<span data-ttu-id="65435-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65435-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65435-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65435-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="65435-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65435-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="65435-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="65435-130">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="delete-a-group-setting"></a><span data-ttu-id="4a1cf-101">Excluir uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="4a1cf-101">Delete a group setting</span></span>

<span data-ttu-id="4a1cf-102">Excluir uma configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-102">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a1cf-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a1cf-103">Permissions</span></span>

<span data-ttu-id="4a1cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a1cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4a1cf-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a1cf-106">Permission type</span></span>      | <span data-ttu-id="4a1cf-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a1cf-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4a1cf-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a1cf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a1cf-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a1cf-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="4a1cf-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a1cf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a1cf-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-111">Not supported.</span></span>    | 
|<span data-ttu-id="4a1cf-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a1cf-112">Application</span></span> | <span data-ttu-id="4a1cf-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a1cf-113">Directory.ReadWrite.All</span></span> | 


## <a name="http-request"></a><span data-ttu-id="4a1cf-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a1cf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="4a1cf-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a1cf-115">Request headers</span></span>

| <span data-ttu-id="4a1cf-116">Nome</span><span class="sxs-lookup"><span data-stu-id="4a1cf-116">Name</span></span> | <span data-ttu-id="4a1cf-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a1cf-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4a1cf-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a1cf-118">Authorization</span></span>  | <span data-ttu-id="4a1cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a1cf-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a1cf-121">Content-Type</span></span>  | <span data-ttu-id="4a1cf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4a1cf-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a1cf-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a1cf-123">Request body</span></span>
<span data-ttu-id="4a1cf-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a1cf-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a1cf-125">Response</span></span>

<span data-ttu-id="4a1cf-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a1cf-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a1cf-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a1cf-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a1cf-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="4a1cf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a1cf-130">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
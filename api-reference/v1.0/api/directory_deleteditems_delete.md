# <a name="permanently-delete-item"></a><span data-ttu-id="559ba-101">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="559ba-101">Permanently delete item</span></span>

<span data-ttu-id="559ba-102">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="559ba-102">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="559ba-103">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="559ba-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="559ba-104">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="559ba-104">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="559ba-105">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="559ba-105">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="559ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="559ba-106">Permissions</span></span>
<span data-ttu-id="559ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="559ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="559ba-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="559ba-109">For users:</span></span>

|<span data-ttu-id="559ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="559ba-110">Permission type</span></span>      | <span data-ttu-id="559ba-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="559ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="559ba-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="559ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="559ba-113">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="559ba-113">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="559ba-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="559ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="559ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="559ba-115">Not supported.</span></span> |
|<span data-ttu-id="559ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="559ba-116">Application</span></span> | <span data-ttu-id="559ba-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="559ba-117">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="559ba-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="559ba-118">For groups:</span></span>

|<span data-ttu-id="559ba-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="559ba-119">Permission type</span></span>      | <span data-ttu-id="559ba-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="559ba-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="559ba-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="559ba-121">Delegated (work or school account)</span></span> | <span data-ttu-id="559ba-122">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="559ba-122">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="559ba-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="559ba-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="559ba-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="559ba-124">Not supported.</span></span>    |
|<span data-ttu-id="559ba-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="559ba-125">Application</span></span> | <span data-ttu-id="559ba-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="559ba-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="559ba-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="559ba-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="559ba-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="559ba-128">Request headers</span></span>
| <span data-ttu-id="559ba-129">Nome</span><span class="sxs-lookup"><span data-stu-id="559ba-129">Name</span></span>       | <span data-ttu-id="559ba-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="559ba-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="559ba-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="559ba-131">Authorization</span></span>  | <span data-ttu-id="559ba-132">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="559ba-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="559ba-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="559ba-133">Accept</span></span>  | <span data-ttu-id="559ba-134">application/json</span><span class="sxs-lookup"><span data-stu-id="559ba-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="559ba-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="559ba-135">Request body</span></span>
<span data-ttu-id="559ba-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="559ba-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="559ba-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="559ba-137">Response</span></span>

<span data-ttu-id="559ba-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="559ba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="559ba-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="559ba-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="559ba-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="559ba-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="559ba-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="559ba-142">Response</span></span>
<span data-ttu-id="559ba-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="559ba-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="restore-deleted-item"></a><span data-ttu-id="d81da-101">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="d81da-101">Restore deleted item</span></span>

<span data-ttu-id="d81da-102">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="d81da-102">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="d81da-103">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d81da-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="d81da-104">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="d81da-104">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="d81da-105">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="d81da-105">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="d81da-106">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="d81da-106">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d81da-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d81da-107">Permissions</span></span>
<span data-ttu-id="d81da-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d81da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="d81da-110">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="d81da-110">For users:</span></span>

|<span data-ttu-id="d81da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d81da-111">Permission type</span></span>      | <span data-ttu-id="d81da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d81da-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d81da-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d81da-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d81da-114">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d81da-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d81da-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d81da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81da-116">Not supported.</span></span> |
|<span data-ttu-id="d81da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d81da-117">Application</span></span> | <span data-ttu-id="d81da-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81da-118">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="d81da-119">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="d81da-119">For groups:</span></span>

|<span data-ttu-id="d81da-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d81da-120">Permission type</span></span>      | <span data-ttu-id="d81da-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d81da-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d81da-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d81da-122">Delegated (work or school account)</span></span> | <span data-ttu-id="d81da-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d81da-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d81da-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d81da-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81da-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81da-125">Not supported.</span></span>    |
|<span data-ttu-id="d81da-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d81da-126">Application</span></span> | <span data-ttu-id="d81da-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81da-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d81da-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d81da-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="d81da-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d81da-129">Request headers</span></span>
| <span data-ttu-id="d81da-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d81da-130">Name</span></span>       | <span data-ttu-id="d81da-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81da-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d81da-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d81da-132">Authorization</span></span>  | <span data-ttu-id="d81da-133">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="d81da-133">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="d81da-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d81da-134">Accept</span></span> | <span data-ttu-id="d81da-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d81da-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d81da-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d81da-136">Request body</span></span>
<span data-ttu-id="d81da-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d81da-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d81da-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81da-138">Response</span></span>

<span data-ttu-id="d81da-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d81da-139">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d81da-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d81da-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d81da-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81da-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="d81da-142">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="d81da-142">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d81da-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81da-143">Response</span></span>
<span data-ttu-id="d81da-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d81da-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
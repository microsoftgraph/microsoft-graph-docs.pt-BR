# <a name="list-deleted-items"></a><span data-ttu-id="6cb3d-101">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="6cb3d-101">List deleted items</span></span>

<span data-ttu-id="6cb3d-102">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6cb3d-102">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="6cb3d-103">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="6cb3d-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cb3d-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cb3d-104">Permissions</span></span>
<span data-ttu-id="6cb3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6cb3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="6cb3d-107">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="6cb3d-107">For users:</span></span>

|<span data-ttu-id="6cb3d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cb3d-108">Permission type</span></span>      | <span data-ttu-id="6cb3d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cb3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb3d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cb3d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb3d-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cb3d-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6cb3d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cb3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb3d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-113">Not supported.</span></span> |
|<span data-ttu-id="6cb3d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cb3d-114">Application</span></span> | <span data-ttu-id="6cb3d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb3d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="6cb3d-116">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="6cb3d-116">For groups:</span></span>

|<span data-ttu-id="6cb3d-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cb3d-117">Permission type</span></span>      | <span data-ttu-id="6cb3d-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cb3d-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb3d-119">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cb3d-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb3d-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cb3d-120">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6cb3d-121">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cb3d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb3d-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-122">Not supported.</span></span>    |
|<span data-ttu-id="6cb3d-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cb3d-123">Application</span></span> | <span data-ttu-id="6cb3d-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cb3d-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cb3d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb3d-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="6cb3d-126">Essa API dá suporte atualmente à recuperação de tipos de objeto de grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-126">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="6cb3d-127">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-127">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="6cb3d-128">Não há suporte para a chamada de GET /directory/deleteditems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-128">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="6cb3d-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6cb3d-129">Optional query parameters</span></span>
<span data-ttu-id="6cb3d-130">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-130">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cb3d-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb3d-131">Request headers</span></span>
| <span data-ttu-id="6cb3d-132">Nome</span><span class="sxs-lookup"><span data-stu-id="6cb3d-132">Name</span></span>      |<span data-ttu-id="6cb3d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb3d-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6cb3d-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cb3d-134">Authorization</span></span>  | <span data-ttu-id="6cb3d-135">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="6cb3d-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="6cb3d-136">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cb3d-136">Accept</span></span>  | <span data-ttu-id="6cb3d-137">application/json</span><span class="sxs-lookup"><span data-stu-id="6cb3d-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cb3d-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb3d-138">Request body</span></span>
<span data-ttu-id="6cb3d-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cb3d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb3d-140">Response</span></span>

<span data-ttu-id="6cb3d-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6cb3d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cb3d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cb3d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb3d-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="6cb3d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb3d-144">Response</span></span>
<span data-ttu-id="6cb3d-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cb3d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
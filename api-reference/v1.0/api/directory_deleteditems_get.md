# <a name="get-deleted-item"></a><span data-ttu-id="7f681-101">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="7f681-101">Get deleted item</span></span>

<span data-ttu-id="7f681-102">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="7f681-102">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="7f681-103">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7f681-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f681-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f681-104">Permissions</span></span>
<span data-ttu-id="7f681-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="7f681-107">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="7f681-107">For users:</span></span>

|<span data-ttu-id="7f681-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f681-108">Permission type</span></span>      | <span data-ttu-id="7f681-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f681-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f681-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f681-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f681-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f681-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="7f681-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f681-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f681-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f681-113">Not supported.</span></span> |
|<span data-ttu-id="7f681-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f681-114">Application</span></span> | <span data-ttu-id="7f681-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f681-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="7f681-116">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="7f681-116">For groups:</span></span>

|<span data-ttu-id="7f681-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f681-117">Permission type</span></span>      | <span data-ttu-id="7f681-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f681-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f681-119">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f681-119">Delegated (work or school account)</span></span> | <span data-ttu-id="7f681-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f681-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7f681-121">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f681-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f681-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f681-122">Not supported.</span></span>    |
|<span data-ttu-id="7f681-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f681-123">Application</span></span> | <span data-ttu-id="7f681-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f681-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f681-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f681-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f681-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f681-126">Optional query parameters</span></span>
<span data-ttu-id="7f681-127">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f681-127">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f681-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f681-128">Request headers</span></span>
| <span data-ttu-id="7f681-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7f681-129">Name</span></span>      |<span data-ttu-id="7f681-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f681-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f681-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f681-131">Authorization</span></span>  | <span data-ttu-id="7f681-132">Código&gt; do portador *Obrigatório*&lt;</span><span class="sxs-lookup"><span data-stu-id="7f681-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="7f681-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f681-133">Accept</span></span>  | <span data-ttu-id="7f681-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7f681-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f681-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f681-135">Request body</span></span>
<span data-ttu-id="7f681-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f681-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f681-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f681-137">Response</span></span>

<span data-ttu-id="7f681-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f681-138">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f681-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f681-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f681-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f681-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="7f681-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f681-141">Response</span></span>
<span data-ttu-id="7f681-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f681-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
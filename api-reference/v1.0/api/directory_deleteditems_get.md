# <a name="get-deleted-item"></a><span data-ttu-id="cbabc-101">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="cbabc-101">Get deleted item</span></span>

<span data-ttu-id="cbabc-102">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="cbabc-102">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="cbabc-103">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="cbabc-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbabc-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbabc-104">Permissions</span></span>
<span data-ttu-id="cbabc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cbabc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="cbabc-107">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="cbabc-107">For users:</span></span>

|<span data-ttu-id="cbabc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbabc-108">Permission type</span></span>      | <span data-ttu-id="cbabc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbabc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbabc-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbabc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbabc-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbabc-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cbabc-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbabc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbabc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbabc-113">Not supported.</span></span> |
|<span data-ttu-id="cbabc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbabc-114">Application</span></span> | <span data-ttu-id="cbabc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbabc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="cbabc-116">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="cbabc-116">For groups:</span></span>

|<span data-ttu-id="cbabc-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbabc-117">Permission type</span></span>      | <span data-ttu-id="cbabc-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbabc-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbabc-119">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbabc-119">Delegated (work or school account)</span></span> | <span data-ttu-id="cbabc-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbabc-120">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cbabc-121">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbabc-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbabc-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbabc-122">Not supported.</span></span>    |
|<span data-ttu-id="cbabc-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbabc-123">Application</span></span> | <span data-ttu-id="cbabc-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbabc-124">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbabc-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbabc-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbabc-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cbabc-126">Optional query parameters</span></span>
<span data-ttu-id="cbabc-127">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cbabc-127">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbabc-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbabc-128">Request headers</span></span>
| <span data-ttu-id="cbabc-129">Nome</span><span class="sxs-lookup"><span data-stu-id="cbabc-129">Name</span></span>      |<span data-ttu-id="cbabc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbabc-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbabc-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbabc-131">Authorization</span></span>  | <span data-ttu-id="cbabc-132">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="cbabc-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="cbabc-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbabc-133">Accept</span></span>  | <span data-ttu-id="cbabc-134">application/json</span><span class="sxs-lookup"><span data-stu-id="cbabc-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbabc-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbabc-135">Request body</span></span>
<span data-ttu-id="cbabc-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbabc-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbabc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbabc-137">Response</span></span>

<span data-ttu-id="cbabc-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbabc-138">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbabc-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbabc-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbabc-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbabc-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="cbabc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbabc-141">Response</span></span>
<span data-ttu-id="cbabc-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbabc-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
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
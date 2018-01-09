# <a name="add-group-owner"></a><span data-ttu-id="fb38e-101">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="fb38e-101">Add group owner</span></span>
<span data-ttu-id="fb38e-p101">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="fb38e-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb38e-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb38e-104">Permissions</span></span>
<span data-ttu-id="fb38e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb38e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb38e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb38e-107">Permission type</span></span>      | <span data-ttu-id="fb38e-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb38e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb38e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb38e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fb38e-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb38e-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb38e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb38e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb38e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb38e-112">Not supported.</span></span>    |
|<span data-ttu-id="fb38e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb38e-113">Application</span></span> | <span data-ttu-id="fb38e-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb38e-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb38e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb38e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fb38e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb38e-116">Request headers</span></span>
| <span data-ttu-id="fb38e-117">Nome</span><span class="sxs-lookup"><span data-stu-id="fb38e-117">Name</span></span>       | <span data-ttu-id="fb38e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb38e-118">Type</span></span> | <span data-ttu-id="fb38e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb38e-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb38e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb38e-120">Authorization</span></span>  | <span data-ttu-id="fb38e-121">string</span><span class="sxs-lookup"><span data-stu-id="fb38e-121">string</span></span>  | <span data-ttu-id="fb38e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb38e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb38e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb38e-124">Request body</span></span>
<span data-ttu-id="fb38e-125">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="fb38e-125">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="fb38e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb38e-126">Response</span></span>
<span data-ttu-id="fb38e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb38e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb38e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb38e-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fb38e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb38e-130">Request</span></span>
<span data-ttu-id="fb38e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb38e-131">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="fb38e-132">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="fb38e-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="fb38e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb38e-133">Response</span></span>
<span data-ttu-id="fb38e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb38e-134">Here is an example of the response.</span></span>
><span data-ttu-id="fb38e-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb38e-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fb38e-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb38e-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="add-group-owner"></a><span data-ttu-id="ecd05-101">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="ecd05-101">Add group owner</span></span>
<span data-ttu-id="ecd05-p101">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="ecd05-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecd05-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecd05-104">Prerequisites</span></span>
<span data-ttu-id="ecd05-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="ecd05-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="ecd05-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecd05-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ecd05-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd05-107">Request headers</span></span>
| <span data-ttu-id="ecd05-108">Nome</span><span class="sxs-lookup"><span data-stu-id="ecd05-108">Name</span></span>       | <span data-ttu-id="ecd05-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecd05-109">Type</span></span> | <span data-ttu-id="ecd05-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd05-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ecd05-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecd05-111">Authorization</span></span>  | <span data-ttu-id="ecd05-112">string</span><span class="sxs-lookup"><span data-stu-id="ecd05-112">string</span></span>  | <span data-ttu-id="ecd05-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecd05-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecd05-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd05-115">Request body</span></span>
<span data-ttu-id="ecd05-116">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ecd05-116">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ecd05-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd05-117">Response</span></span>

<span data-ttu-id="ecd05-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecd05-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecd05-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecd05-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ecd05-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd05-121">Request</span></span>
<span data-ttu-id="ecd05-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecd05-122">Here is an example of the request.</span></span>
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
<span data-ttu-id="ecd05-123">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ecd05-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="ecd05-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd05-124">Response</span></span>
<span data-ttu-id="ecd05-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecd05-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

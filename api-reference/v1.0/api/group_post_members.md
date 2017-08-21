# <a name="add-member"></a><span data-ttu-id="e3410-101">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="e3410-101">Add member</span></span>

<span data-ttu-id="e3410-p101">Use esta API para adicionar um membro a um grupo do Office 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação **members**. É possível adicionar usuários ou outros grupos. Importante: é possível adicionar somente usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e3410-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3410-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3410-105">Prerequisites</span></span>
<span data-ttu-id="e3410-106">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="e3410-106">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e3410-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3410-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e3410-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3410-108">Request headers</span></span>
| <span data-ttu-id="e3410-109">Nome</span><span class="sxs-lookup"><span data-stu-id="e3410-109">Name</span></span>       | <span data-ttu-id="e3410-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3410-110">Type</span></span> | <span data-ttu-id="e3410-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3410-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3410-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3410-112">Authorization</span></span>  | <span data-ttu-id="e3410-113">string</span><span class="sxs-lookup"><span data-stu-id="e3410-113">string</span></span>  | <span data-ttu-id="e3410-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3410-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3410-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3410-116">Request body</span></span>
<span data-ttu-id="e3410-117">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="e3410-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e3410-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3410-118">Response</span></span>

<span data-ttu-id="e3410-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3410-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3410-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3410-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3410-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3410-122">Request</span></span>
<span data-ttu-id="e3410-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3410-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="e3410-124">No corpo da solicitação, forneça uma representação JSON da `id` do objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="e3410-124">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="e3410-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3410-125">Response</span></span>
<span data-ttu-id="e3410-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3410-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="assign-a-manager"></a><span data-ttu-id="141bd-101">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="141bd-101">Assign a manager</span></span>

<span data-ttu-id="141bd-102">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="141bd-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="141bd-103">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="141bd-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="141bd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="141bd-104">Prerequisites</span></span>
<span data-ttu-id="141bd-105">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="141bd-105">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="141bd-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="141bd-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="141bd-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="141bd-107">Request headers</span></span>
| <span data-ttu-id="141bd-108">Nome</span><span class="sxs-lookup"><span data-stu-id="141bd-108">Name</span></span>       | <span data-ttu-id="141bd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="141bd-109">Type</span></span> | <span data-ttu-id="141bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="141bd-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="141bd-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="141bd-111">Authorization</span></span>  | <span data-ttu-id="141bd-112">string</span><span class="sxs-lookup"><span data-stu-id="141bd-112">string</span></span>  | <span data-ttu-id="141bd-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="141bd-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="141bd-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="141bd-115">Request body</span></span>
<span data-ttu-id="141bd-116">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="141bd-116">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="141bd-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="141bd-117">Response</span></span>

<span data-ttu-id="141bd-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="141bd-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="141bd-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="141bd-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="141bd-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="141bd-121">Request</span></span>
<span data-ttu-id="141bd-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="141bd-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="141bd-123">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="141bd-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="141bd-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="141bd-124">Response</span></span>
<span data-ttu-id="141bd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="141bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

# <a name="assign-a-manager"></a><span data-ttu-id="f5507-101">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="f5507-101">Assign a manager</span></span>

<span data-ttu-id="f5507-102">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f5507-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="f5507-103">Observação: Não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="f5507-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5507-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5507-104">Permissions</span></span>
<span data-ttu-id="f5507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5507-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5507-107">Permission type</span></span>      | <span data-ttu-id="f5507-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5507-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f5507-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5507-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f5507-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5507-110">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="f5507-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5507-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5507-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5507-112">Not supported.</span></span>    | 
|<span data-ttu-id="f5507-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5507-113">Application</span></span> | <span data-ttu-id="f5507-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5507-114">Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f5507-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5507-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f5507-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5507-116">Request headers</span></span>
| <span data-ttu-id="f5507-117">Nome</span><span class="sxs-lookup"><span data-stu-id="f5507-117">Name</span></span>       | <span data-ttu-id="f5507-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5507-118">Type</span></span> | <span data-ttu-id="f5507-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5507-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5507-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5507-120">Authorization</span></span>  | <span data-ttu-id="f5507-121">string</span><span class="sxs-lookup"><span data-stu-id="f5507-121">string</span></span>  | <span data-ttu-id="f5507-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5507-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5507-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5507-124">Request body</span></span>
<span data-ttu-id="f5507-125">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="f5507-125">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f5507-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5507-126">Response</span></span>

<span data-ttu-id="f5507-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5507-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5507-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5507-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5507-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5507-130">Request</span></span>
<span data-ttu-id="f5507-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5507-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="f5507-132">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="f5507-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="f5507-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5507-133">Response</span></span>
<span data-ttu-id="f5507-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5507-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

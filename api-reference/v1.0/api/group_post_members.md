# <a name="add-member"></a><span data-ttu-id="a1c4f-101">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="a1c4f-101">Add member</span></span>
<span data-ttu-id="a1c4f-102">Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-102">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="a1c4f-103">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-103">You can add users or other groups.</span></span> <span data-ttu-id="a1c4f-104">Importante: só é possível adicionar usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-104">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1c4f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1c4f-105">Permissions</span></span>
<span data-ttu-id="a1c4f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1c4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1c4f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1c4f-108">Permission type</span></span>      | <span data-ttu-id="a1c4f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1c4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1c4f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1c4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a1c4f-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1c4f-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1c4f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1c4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c4f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-113">Not supported.</span></span>    |
|<span data-ttu-id="a1c4f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1c4f-114">Application</span></span> | <span data-ttu-id="a1c4f-115">Group.ReadWrite.All e User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c4f-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1c4f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c4f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a1c4f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c4f-117">Request headers</span></span>
| <span data-ttu-id="a1c4f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a1c4f-118">Name</span></span>       | <span data-ttu-id="a1c4f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1c4f-119">Type</span></span> | <span data-ttu-id="a1c4f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c4f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1c4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1c4f-121">Authorization</span></span>  | <span data-ttu-id="a1c4f-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1c4f-122">string</span></span>  | <span data-ttu-id="a1c4f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1c4f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c4f-125">Request body</span></span>
<span data-ttu-id="a1c4f-126">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a1c4f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c4f-127">Response</span></span>
<span data-ttu-id="a1c4f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1c4f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1c4f-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a1c4f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c4f-131">Request</span></span>
<span data-ttu-id="a1c4f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="a1c4f-133">No corpo da solicitação, forneça uma representação JSON da `id` do objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-133">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="a1c4f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c4f-134">Response</span></span>
<span data-ttu-id="a1c4f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-135">The following is an example of the response.</span></span>
><span data-ttu-id="a1c4f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1c4f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
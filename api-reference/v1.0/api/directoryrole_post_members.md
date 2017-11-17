# <a name="add-directory-role-member"></a><span data-ttu-id="43b88-101">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="43b88-101">Add directory role member</span></span>

<span data-ttu-id="43b88-102">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="43b88-102">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="43b88-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="43b88-103">Permissions</span></span>
<span data-ttu-id="43b88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43b88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43b88-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43b88-106">Permission type</span></span>      | <span data-ttu-id="43b88-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43b88-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43b88-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43b88-108">Delegated (work or school account)</span></span> | <span data-ttu-id="43b88-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43b88-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43b88-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43b88-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43b88-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43b88-111">Not supported.</span></span>    |
|<span data-ttu-id="43b88-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43b88-112">Application</span></span> | <span data-ttu-id="43b88-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43b88-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43b88-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43b88-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="43b88-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43b88-115">Request headers</span></span>
| <span data-ttu-id="43b88-116">Nome</span><span class="sxs-lookup"><span data-stu-id="43b88-116">Name</span></span>       | <span data-ttu-id="43b88-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="43b88-117">Type</span></span> | <span data-ttu-id="43b88-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="43b88-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43b88-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="43b88-119">Authorization</span></span>  | <span data-ttu-id="43b88-120">string</span><span class="sxs-lookup"><span data-stu-id="43b88-120">string</span></span>  | <span data-ttu-id="43b88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43b88-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43b88-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43b88-123">Content-Type</span></span>  | <span data-ttu-id="43b88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="43b88-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43b88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43b88-125">Request body</span></span>
<span data-ttu-id="43b88-126">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="43b88-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="43b88-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="43b88-127">Response</span></span>

<span data-ttu-id="43b88-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="43b88-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43b88-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43b88-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43b88-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43b88-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="43b88-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="43b88-131">Response</span></span>
<span data-ttu-id="43b88-132">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="43b88-132">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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
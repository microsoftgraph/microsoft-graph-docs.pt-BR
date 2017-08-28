# <a name="delete-directoryobject"></a><span data-ttu-id="fee4b-101">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="fee4b-101">Delete directoryObject</span></span>

<span data-ttu-id="fee4b-102">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="fee4b-102">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="fee4b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="fee4b-103">Permissions</span></span>
<span data-ttu-id="fee4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fee4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="fee4b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fee4b-106">Permission type</span></span>      | <span data-ttu-id="fee4b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fee4b-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fee4b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fee4b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fee4b-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fee4b-109">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="fee4b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fee4b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fee4b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee4b-111">Not supported.</span></span>    | 
|<span data-ttu-id="fee4b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fee4b-112">Application</span></span> | <span data-ttu-id="fee4b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee4b-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fee4b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fee4b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fee4b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fee4b-115">Request headers</span></span>
| <span data-ttu-id="fee4b-116">Nome</span><span class="sxs-lookup"><span data-stu-id="fee4b-116">Name</span></span>       | <span data-ttu-id="fee4b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee4b-117">Type</span></span> | <span data-ttu-id="fee4b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee4b-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fee4b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="fee4b-119">Authorization</span></span>  | <span data-ttu-id="fee4b-120">string</span><span class="sxs-lookup"><span data-stu-id="fee4b-120">string</span></span>  | <span data-ttu-id="fee4b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fee4b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fee4b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fee4b-123">Request body</span></span>
<span data-ttu-id="fee4b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fee4b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fee4b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee4b-125">Response</span></span>

<span data-ttu-id="fee4b-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fee4b-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fee4b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fee4b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fee4b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fee4b-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="fee4b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee4b-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
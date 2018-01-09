# <a name="remove-owner"></a><span data-ttu-id="49ab0-101">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="49ab0-101">Remove owner</span></span>
<span data-ttu-id="49ab0-102">Use esta API para remover um proprietário de um grupo do Office 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="49ab0-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="49ab0-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="49ab0-103">Permissions</span></span>
<span data-ttu-id="49ab0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="49ab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="49ab0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49ab0-106">Permission type</span></span>      | <span data-ttu-id="49ab0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49ab0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49ab0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49ab0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="49ab0-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49ab0-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49ab0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49ab0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49ab0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49ab0-111">Not supported.</span></span>    |
|<span data-ttu-id="49ab0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49ab0-112">Application</span></span> | <span data-ttu-id="49ab0-113">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ab0-113">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49ab0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49ab0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="49ab0-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49ab0-115">Request headers</span></span>
| <span data-ttu-id="49ab0-116">Nome</span><span class="sxs-lookup"><span data-stu-id="49ab0-116">Name</span></span>       | <span data-ttu-id="49ab0-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="49ab0-117">Type</span></span> | <span data-ttu-id="49ab0-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="49ab0-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49ab0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="49ab0-119">Authorization</span></span>  | <span data-ttu-id="49ab0-120">string</span><span class="sxs-lookup"><span data-stu-id="49ab0-120">string</span></span>  | <span data-ttu-id="49ab0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49ab0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49ab0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49ab0-123">Request body</span></span>
<span data-ttu-id="49ab0-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49ab0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49ab0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ab0-125">Response</span></span>
<span data-ttu-id="49ab0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49ab0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49ab0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49ab0-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="49ab0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49ab0-129">Request</span></span>
<span data-ttu-id="49ab0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49ab0-130">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="49ab0-131">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="49ab0-131">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="49ab0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ab0-132">Response</span></span>
<span data-ttu-id="49ab0-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49ab0-133">Here is an example of the response.</span></span>
><span data-ttu-id="49ab0-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="49ab0-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49ab0-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49ab0-135">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

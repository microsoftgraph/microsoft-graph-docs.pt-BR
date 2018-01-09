# <a name="remove-member"></a><span data-ttu-id="233fc-101">Remover membro</span><span class="sxs-lookup"><span data-stu-id="233fc-101">Remove member</span></span>
<span data-ttu-id="233fc-p101">Use esta API para remover um membro de um grupo do Office 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação **members**. É possível remover usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="233fc-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="233fc-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="233fc-104">Permissions</span></span>
<span data-ttu-id="233fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="233fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="233fc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="233fc-107">Permission type</span></span>      | <span data-ttu-id="233fc-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="233fc-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233fc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="233fc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="233fc-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="233fc-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="233fc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="233fc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="233fc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="233fc-112">Not supported.</span></span>    |
|<span data-ttu-id="233fc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="233fc-113">Application</span></span> | <span data-ttu-id="233fc-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233fc-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="233fc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="233fc-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="233fc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="233fc-116">Request headers</span></span>
| <span data-ttu-id="233fc-117">Nome</span><span class="sxs-lookup"><span data-stu-id="233fc-117">Name</span></span>       | <span data-ttu-id="233fc-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="233fc-118">Type</span></span> | <span data-ttu-id="233fc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="233fc-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="233fc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="233fc-120">Authorization</span></span>  | <span data-ttu-id="233fc-121">string</span><span class="sxs-lookup"><span data-stu-id="233fc-121">string</span></span>  | <span data-ttu-id="233fc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="233fc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="233fc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="233fc-124">Request body</span></span>
<span data-ttu-id="233fc-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="233fc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="233fc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="233fc-126">Response</span></span>
<span data-ttu-id="233fc-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="233fc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="233fc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="233fc-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="233fc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="233fc-130">Request</span></span>
<span data-ttu-id="233fc-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="233fc-131">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="233fc-132">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="233fc-132">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="233fc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="233fc-133">Response</span></span>
<span data-ttu-id="233fc-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="233fc-134">Here is an example of the response.</span></span>
><span data-ttu-id="233fc-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="233fc-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="233fc-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="233fc-136">All the properties will be returned from an actual call.</span></span>
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
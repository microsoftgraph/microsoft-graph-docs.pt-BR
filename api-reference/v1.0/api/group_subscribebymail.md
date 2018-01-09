# <a name="group-subscribebymail"></a><span data-ttu-id="47bb0-101">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="47bb0-101">group: subscribeByMail</span></span>

<span data-ttu-id="47bb0-p101">Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="47bb0-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="47bb0-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="47bb0-104">Permissions</span></span>
<span data-ttu-id="47bb0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47bb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47bb0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47bb0-107">Permission type</span></span>      | <span data-ttu-id="47bb0-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47bb0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47bb0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47bb0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="47bb0-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47bb0-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47bb0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47bb0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47bb0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47bb0-112">Not supported.</span></span>    |
|<span data-ttu-id="47bb0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47bb0-113">Application</span></span> | <span data-ttu-id="47bb0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47bb0-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47bb0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47bb0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="47bb0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47bb0-116">Request headers</span></span>
| <span data-ttu-id="47bb0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47bb0-117">Header</span></span>       | <span data-ttu-id="47bb0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="47bb0-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47bb0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="47bb0-119">Authorization</span></span>  | <span data-ttu-id="47bb0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47bb0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47bb0-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47bb0-122">Request body</span></span>
<span data-ttu-id="47bb0-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47bb0-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47bb0-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bb0-124">Response</span></span>
<span data-ttu-id="47bb0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47bb0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47bb0-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47bb0-127">Example</span></span>
<span data-ttu-id="47bb0-128">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="47bb0-128">Here is an example of how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="47bb0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47bb0-129">Request</span></span>
<span data-ttu-id="47bb0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47bb0-130">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="47bb0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bb0-131">Response</span></span>
<span data-ttu-id="47bb0-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47bb0-132">Here is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
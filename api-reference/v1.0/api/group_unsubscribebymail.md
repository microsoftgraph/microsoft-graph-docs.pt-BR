# <a name="group-unsubscribebymail"></a><span data-ttu-id="5c67a-101">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="5c67a-101">group: unsubscribeByMail</span></span>
<span data-ttu-id="5c67a-p101">Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="5c67a-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5c67a-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c67a-104">Permissions</span></span>
<span data-ttu-id="5c67a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c67a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5c67a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c67a-107">Permission type</span></span>      | <span data-ttu-id="5c67a-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c67a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c67a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c67a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5c67a-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c67a-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c67a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c67a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c67a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c67a-112">Not supported.</span></span>    |
|<span data-ttu-id="5c67a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c67a-113">Application</span></span> | <span data-ttu-id="5c67a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c67a-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c67a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c67a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="5c67a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c67a-116">Request headers</span></span>
| <span data-ttu-id="5c67a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c67a-117">Header</span></span>       | <span data-ttu-id="5c67a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="5c67a-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c67a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c67a-119">Authorization</span></span>  | <span data-ttu-id="5c67a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c67a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c67a-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c67a-122">Request body</span></span>
<span data-ttu-id="5c67a-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c67a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c67a-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c67a-124">Response</span></span>
<span data-ttu-id="5c67a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c67a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c67a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c67a-127">Example</span></span>
<span data-ttu-id="5c67a-128">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5c67a-128">Here is an example of how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="5c67a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c67a-129">Request</span></span>
<span data-ttu-id="5c67a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c67a-130">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

#### <a name="response"></a><span data-ttu-id="5c67a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c67a-131">Response</span></span>
<span data-ttu-id="5c67a-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c67a-132">Here is an example of the response.</span></span> 
><span data-ttu-id="5c67a-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c67a-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5c67a-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c67a-134">All the properties will be returned from an actual call.</span></span>
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

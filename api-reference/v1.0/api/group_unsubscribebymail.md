# <a name="group-unsubscribebymail"></a><span data-ttu-id="26ddf-101">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="26ddf-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="26ddf-p101">Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="26ddf-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="permissions"></a><span data-ttu-id="26ddf-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="26ddf-104">Permissions</span></span>
<span data-ttu-id="26ddf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26ddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="26ddf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26ddf-107">Permission type</span></span>      | <span data-ttu-id="26ddf-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26ddf-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="26ddf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26ddf-109">Delegated (work or school account)</span></span> | <span data-ttu-id="26ddf-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ddf-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="26ddf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26ddf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26ddf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26ddf-112">Not supported.</span></span>    | 
|<span data-ttu-id="26ddf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26ddf-113">Application</span></span> | <span data-ttu-id="26ddf-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ddf-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="26ddf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26ddf-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="26ddf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26ddf-116">Request headers</span></span>
| <span data-ttu-id="26ddf-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26ddf-117">Header</span></span>       | <span data-ttu-id="26ddf-118">Valor</span><span class="sxs-lookup"><span data-stu-id="26ddf-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26ddf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="26ddf-119">Authorization</span></span>  | <span data-ttu-id="26ddf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26ddf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26ddf-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26ddf-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="26ddf-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ddf-123">Response</span></span>
<span data-ttu-id="26ddf-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ddf-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26ddf-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26ddf-126">Example</span></span>
<span data-ttu-id="26ddf-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="26ddf-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="26ddf-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26ddf-128">Request</span></span>
<span data-ttu-id="26ddf-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ddf-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="26ddf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ddf-130">Response</span></span>
<span data-ttu-id="26ddf-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ddf-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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

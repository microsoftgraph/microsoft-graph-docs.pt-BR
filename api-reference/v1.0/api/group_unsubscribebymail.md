# <a name="group-unsubscribebymail"></a><span data-ttu-id="eaff0-101">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="eaff0-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="eaff0-p101">Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="eaff0-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="eaff0-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eaff0-104">Prerequisites</span></span>
<span data-ttu-id="eaff0-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="eaff0-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="eaff0-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaff0-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="eaff0-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaff0-107">Request headers</span></span>
| <span data-ttu-id="eaff0-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eaff0-108">Header</span></span>       | <span data-ttu-id="eaff0-109">Valor</span><span class="sxs-lookup"><span data-stu-id="eaff0-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eaff0-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaff0-110">Authorization</span></span>  | <span data-ttu-id="eaff0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaff0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eaff0-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaff0-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="eaff0-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaff0-114">Response</span></span>

<span data-ttu-id="eaff0-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaff0-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaff0-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaff0-117">Example</span></span>
<span data-ttu-id="eaff0-118">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eaff0-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eaff0-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaff0-119">Request</span></span>
<span data-ttu-id="eaff0-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaff0-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="eaff0-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaff0-121">Response</span></span>
<span data-ttu-id="eaff0-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaff0-122">Here is an example of the response.</span></span> 
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

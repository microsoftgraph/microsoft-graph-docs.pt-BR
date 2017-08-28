# <a name="group-resetunseencount"></a><span data-ttu-id="63afc-101">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="63afc-101">group: resetUnseenCount</span></span>

<span data-ttu-id="63afc-p101">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="63afc-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="63afc-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="63afc-104">Permissions</span></span>
<span data-ttu-id="63afc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63afc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63afc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63afc-107">Permission type</span></span>      | <span data-ttu-id="63afc-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63afc-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="63afc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63afc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="63afc-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63afc-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="63afc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63afc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63afc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63afc-112">Not supported.</span></span>    | 
|<span data-ttu-id="63afc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63afc-113">Application</span></span> | <span data-ttu-id="63afc-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63afc-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="63afc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63afc-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="63afc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63afc-116">Request headers</span></span>
| <span data-ttu-id="63afc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63afc-117">Header</span></span>       | <span data-ttu-id="63afc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="63afc-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63afc-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="63afc-119">Authorization</span></span>  | <span data-ttu-id="63afc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63afc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63afc-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63afc-122">Request body</span></span>
<span data-ttu-id="63afc-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63afc-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63afc-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="63afc-124">Response</span></span>

<span data-ttu-id="63afc-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63afc-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63afc-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63afc-127">Example</span></span>
<span data-ttu-id="63afc-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="63afc-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63afc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63afc-129">Request</span></span>
<span data-ttu-id="63afc-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63afc-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="63afc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="63afc-131">Response</span></span>
<span data-ttu-id="63afc-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63afc-132">Here is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

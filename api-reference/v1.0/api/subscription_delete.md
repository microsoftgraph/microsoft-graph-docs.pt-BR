# <a name="delete-subscription"></a><span data-ttu-id="f5e08-101">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="f5e08-101">Delete subscription</span></span>

<span data-ttu-id="f5e08-102">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="f5e08-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5e08-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5e08-103">Permissions</span></span>

<span data-ttu-id="f5e08-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5e08-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f5e08-106">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="f5e08-106">Resource type / Item</span></span>        | <span data-ttu-id="f5e08-107">Permissão</span><span class="sxs-lookup"><span data-stu-id="f5e08-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="f5e08-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="f5e08-108">Contacts</span></span>                    | <span data-ttu-id="f5e08-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f5e08-109">Contacts.Read</span></span>       |
| <span data-ttu-id="f5e08-110">Conversas</span><span class="sxs-lookup"><span data-stu-id="f5e08-110">Conversations</span></span>               | <span data-ttu-id="f5e08-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5e08-111">Group.Read.All</span></span>      |
| <span data-ttu-id="f5e08-112">Eventos</span><span class="sxs-lookup"><span data-stu-id="f5e08-112">Events</span></span>                      | <span data-ttu-id="f5e08-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f5e08-113">Calendars.Read</span></span>      |
| <span data-ttu-id="f5e08-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="f5e08-114">Messages</span></span>                    | <span data-ttu-id="f5e08-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f5e08-115">Mail.Read</span></span>           |
| <span data-ttu-id="f5e08-116">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="f5e08-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="f5e08-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5e08-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="f5e08-118">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="f5e08-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="f5e08-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5e08-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5e08-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e08-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="f5e08-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e08-121">Request headers</span></span>
| <span data-ttu-id="f5e08-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f5e08-122">Name</span></span>       | <span data-ttu-id="f5e08-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5e08-123">Type</span></span> | <span data-ttu-id="f5e08-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e08-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5e08-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5e08-125">Authorization</span></span>  | <span data-ttu-id="f5e08-126">string</span><span class="sxs-lookup"><span data-stu-id="f5e08-126">string</span></span>  | <span data-ttu-id="f5e08-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5e08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5e08-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e08-129">Request body</span></span>
<span data-ttu-id="f5e08-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5e08-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5e08-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e08-131">Response</span></span>

<span data-ttu-id="f5e08-132">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5e08-132">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="f5e08-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5e08-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5e08-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e08-134">Request</span></span>
<span data-ttu-id="f5e08-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5e08-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="f5e08-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e08-136">Response</span></span>
<span data-ttu-id="f5e08-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5e08-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

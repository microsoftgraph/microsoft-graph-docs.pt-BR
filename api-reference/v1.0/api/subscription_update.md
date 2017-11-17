# <a name="update-subscription"></a><span data-ttu-id="d86ad-101">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="d86ad-101">Update subscription</span></span>

<span data-ttu-id="d86ad-102">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="d86ad-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="d86ad-p101">As assinaturas a recursos expiram nas datas prescritas pelos tipos de recursos individuais.  Para não perder as notificações, as assinaturas devem ser renovadas bem antes de sua data de vencimento.  Consulte [subscription](../resources/subscription.md) para saber mais sobre datas de vencimento individuais.</span><span class="sxs-lookup"><span data-stu-id="d86ad-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="permissions"></a><span data-ttu-id="d86ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d86ad-106">Permissions</span></span>

<span data-ttu-id="d86ad-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d86ad-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d86ad-109">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="d86ad-109">Resource type / Item</span></span>        | <span data-ttu-id="d86ad-110">Permissão</span><span class="sxs-lookup"><span data-stu-id="d86ad-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="d86ad-111">Contatos</span><span class="sxs-lookup"><span data-stu-id="d86ad-111">Contacts</span></span>                    | <span data-ttu-id="d86ad-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d86ad-112">Contacts.Read</span></span>       |
| <span data-ttu-id="d86ad-113">Conversas</span><span class="sxs-lookup"><span data-stu-id="d86ad-113">Conversations</span></span>               | <span data-ttu-id="d86ad-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d86ad-114">Group.Read.All</span></span>      |
| <span data-ttu-id="d86ad-115">Eventos</span><span class="sxs-lookup"><span data-stu-id="d86ad-115">Events</span></span>                      | <span data-ttu-id="d86ad-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d86ad-116">Calendars.Read</span></span>      |
| <span data-ttu-id="d86ad-117">Mensagens</span><span class="sxs-lookup"><span data-stu-id="d86ad-117">Messages</span></span>                    | <span data-ttu-id="d86ad-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d86ad-118">Mail.Read</span></span>           |
| <span data-ttu-id="d86ad-119">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="d86ad-119">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d86ad-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d86ad-120">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d86ad-121">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="d86ad-121">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="d86ad-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86ad-122">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d86ad-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d86ad-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="d86ad-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d86ad-124">Request headers</span></span>
| <span data-ttu-id="d86ad-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d86ad-125">Name</span></span>       | <span data-ttu-id="d86ad-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d86ad-126">Type</span></span> | <span data-ttu-id="d86ad-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d86ad-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d86ad-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d86ad-128">Authorization</span></span>  | <span data-ttu-id="d86ad-129">string</span><span class="sxs-lookup"><span data-stu-id="d86ad-129">string</span></span>  | <span data-ttu-id="d86ad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d86ad-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d86ad-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d86ad-132">Response</span></span>

<span data-ttu-id="d86ad-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d86ad-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d86ad-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d86ad-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d86ad-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d86ad-135">Request</span></span>
<span data-ttu-id="d86ad-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d86ad-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="d86ad-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d86ad-137">Response</span></span>
<span data-ttu-id="d86ad-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d86ad-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="update-subscription"></a><span data-ttu-id="b5001-101">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="b5001-101">Update subscription</span></span>

<span data-ttu-id="b5001-102">Renove uma assinatura ampliando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="b5001-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="b5001-103">Assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="b5001-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="b5001-104">Para não deixar de receber notificações, um aplicativo deve renovar sua assinatura com uma boa antecedência da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="b5001-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="b5001-105">Consulte [assinatura](../resources/subscription.md) para o comprimento máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="b5001-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5001-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5001-106">Permissions</span></span>

<span data-ttu-id="b5001-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5001-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b5001-109">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="b5001-109">Resource type / Item</span></span>        | <span data-ttu-id="b5001-110">Permissão</span><span class="sxs-lookup"><span data-stu-id="b5001-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b5001-111">Contatos</span><span class="sxs-lookup"><span data-stu-id="b5001-111">Contacts</span></span>                    | <span data-ttu-id="b5001-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b5001-112">Contacts.Read</span></span>       |
| <span data-ttu-id="b5001-113">Conversas</span><span class="sxs-lookup"><span data-stu-id="b5001-113">Conversations</span></span>               | <span data-ttu-id="b5001-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5001-114">Group.Read.All</span></span>      |
| <span data-ttu-id="b5001-115">Eventos</span><span class="sxs-lookup"><span data-stu-id="b5001-115">Events</span></span>                      | <span data-ttu-id="b5001-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b5001-116">Calendars.Read</span></span>      |
| <span data-ttu-id="b5001-117">Mensagens</span><span class="sxs-lookup"><span data-stu-id="b5001-117">Messages</span></span>                    | <span data-ttu-id="b5001-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b5001-118">Mail.Read</span></span>           |
| <span data-ttu-id="b5001-119">Grupos</span><span class="sxs-lookup"><span data-stu-id="b5001-119">Groups</span></span>                      | <span data-ttu-id="b5001-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5001-120">Group.Read.All</span></span>      |
| <span data-ttu-id="b5001-121">Usuários</span><span class="sxs-lookup"><span data-stu-id="b5001-121">Users</span></span>                       | <span data-ttu-id="b5001-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5001-122">User.Read.All</span></span>       |
| <span data-ttu-id="b5001-123">Unidade (OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="b5001-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b5001-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5001-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b5001-125">Unidades (unidades e conteúdo compartilhado do SharePoint)</span><span class="sxs-lookup"><span data-stu-id="b5001-125">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="b5001-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5001-126">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5001-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5001-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5001-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5001-128">Request headers</span></span>

| <span data-ttu-id="b5001-129">Nome</span><span class="sxs-lookup"><span data-stu-id="b5001-129">Name</span></span>       | <span data-ttu-id="b5001-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5001-130">Type</span></span> | <span data-ttu-id="b5001-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5001-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b5001-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5001-132">Authorization</span></span>  | <span data-ttu-id="b5001-133">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5001-133">string</span></span>  | <span data-ttu-id="b5001-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5001-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b5001-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5001-136">Response</span></span>

<span data-ttu-id="b5001-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5001-137">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5001-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5001-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5001-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5001-139">Request</span></span>

<span data-ttu-id="b5001-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5001-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="b5001-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5001-141">Response</span></span>

<span data-ttu-id="b5001-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5001-142">Here is an example of the response.</span></span>
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

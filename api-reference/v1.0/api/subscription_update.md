# <a name="update-subscription"></a><span data-ttu-id="d05be-101">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="d05be-101">Update subscription</span></span>

<span data-ttu-id="d05be-102">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="d05be-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="d05be-p101">As assinaturas a recursos expiram nas datas prescritas pelos tipos de recursos individuais.  Para não perder as notificações, as assinaturas devem ser renovadas bem antes de sua data de vencimento.  Consulte [subscription](../resources/subscription.md) para saber mais sobre datas de vencimento individuais.</span><span class="sxs-lookup"><span data-stu-id="d05be-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d05be-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d05be-106">Prerequisites</span></span>

<span data-ttu-id="d05be-107">A tabela a seguir lista a permissão sugerida necessária para cada recurso.</span><span class="sxs-lookup"><span data-stu-id="d05be-107">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="d05be-108">Tipo de recurso / item</span><span class="sxs-lookup"><span data-stu-id="d05be-108">Resource type / Item</span></span>        | <span data-ttu-id="d05be-109">Escopo</span><span class="sxs-lookup"><span data-stu-id="d05be-109">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="d05be-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="d05be-110">Contacts</span></span>                    | <span data-ttu-id="d05be-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d05be-111">Contacts.Read</span></span>       |
| <span data-ttu-id="d05be-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="d05be-112">Conversations</span></span>               | <span data-ttu-id="d05be-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d05be-113">Group.Read.All</span></span>      |
| <span data-ttu-id="d05be-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="d05be-114">Events</span></span>                      | <span data-ttu-id="d05be-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d05be-115">Calendars.Read</span></span>      |
| <span data-ttu-id="d05be-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="d05be-116">Messages</span></span>                    | <span data-ttu-id="d05be-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d05be-117">Mail.Read</span></span>           |
| <span data-ttu-id="d05be-118">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="d05be-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d05be-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d05be-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d05be-120">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="d05be-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="d05be-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05be-121">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d05be-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d05be-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="d05be-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d05be-123">Request headers</span></span>
| <span data-ttu-id="d05be-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d05be-124">Name</span></span>       | <span data-ttu-id="d05be-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d05be-125">Type</span></span> | <span data-ttu-id="d05be-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d05be-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d05be-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d05be-127">Authorization</span></span>  | <span data-ttu-id="d05be-128">string</span><span class="sxs-lookup"><span data-stu-id="d05be-128">string</span></span>  | <span data-ttu-id="d05be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d05be-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d05be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d05be-131">Response</span></span>

<span data-ttu-id="d05be-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d05be-132">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d05be-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d05be-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d05be-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d05be-134">Request</span></span>
<span data-ttu-id="d05be-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d05be-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d05be-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d05be-136">Response</span></span>
<span data-ttu-id="d05be-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d05be-137">Here is an example of the response.</span></span>
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

# <a name="get-subscription"></a><span data-ttu-id="075d7-101">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="075d7-101">Get subscription</span></span>

<span data-ttu-id="075d7-102">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="075d7-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="permissions"></a><span data-ttu-id="075d7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="075d7-103">Permissions</span></span>

<span data-ttu-id="075d7-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="075d7-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="075d7-106">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="075d7-106">Resource type / Item</span></span>        | <span data-ttu-id="075d7-107">Permissão</span><span class="sxs-lookup"><span data-stu-id="075d7-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="075d7-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="075d7-108">Contacts</span></span>                    | <span data-ttu-id="075d7-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="075d7-109">Contacts.Read</span></span>       |
| <span data-ttu-id="075d7-110">Conversas</span><span class="sxs-lookup"><span data-stu-id="075d7-110">Conversations</span></span>               | <span data-ttu-id="075d7-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="075d7-111">Group.Read.All</span></span>      |
| <span data-ttu-id="075d7-112">Eventos</span><span class="sxs-lookup"><span data-stu-id="075d7-112">Events</span></span>                      | <span data-ttu-id="075d7-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="075d7-113">Calendars.Read</span></span>      |
| <span data-ttu-id="075d7-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="075d7-114">Messages</span></span>                    | <span data-ttu-id="075d7-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="075d7-115">Mail.Read</span></span>           |
| <span data-ttu-id="075d7-116">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="075d7-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="075d7-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="075d7-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="075d7-118">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="075d7-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="075d7-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="075d7-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="075d7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="075d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="075d7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="075d7-121">Optional query parameters</span></span>
<span data-ttu-id="075d7-122">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="075d7-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="075d7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="075d7-123">Request headers</span></span>
| <span data-ttu-id="075d7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="075d7-124">Name</span></span>       | <span data-ttu-id="075d7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="075d7-125">Type</span></span> | <span data-ttu-id="075d7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="075d7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="075d7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="075d7-127">Authorization</span></span>  | <span data-ttu-id="075d7-128">string</span><span class="sxs-lookup"><span data-stu-id="075d7-128">string</span></span>  | <span data-ttu-id="075d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="075d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="075d7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="075d7-131">Request body</span></span>
<span data-ttu-id="075d7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="075d7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="075d7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="075d7-133">Response</span></span>

<span data-ttu-id="075d7-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="075d7-134">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="075d7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="075d7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="075d7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="075d7-136">Request</span></span>
<span data-ttu-id="075d7-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="075d7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="075d7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="075d7-138">Response</span></span>
<span data-ttu-id="075d7-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="075d7-139">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

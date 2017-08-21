# <a name="get-subscription"></a><span data-ttu-id="d606b-101">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="d606b-101">Get subscription</span></span>

<span data-ttu-id="d606b-102">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d606b-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d606b-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d606b-103">Prerequisites</span></span>

<span data-ttu-id="d606b-104">A tabela a seguir lista a permissão sugerida necessária para cada recurso.</span><span class="sxs-lookup"><span data-stu-id="d606b-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="d606b-105">Tipo de recurso / item</span><span class="sxs-lookup"><span data-stu-id="d606b-105">Resource type / Item</span></span>        | <span data-ttu-id="d606b-106">Escopo</span><span class="sxs-lookup"><span data-stu-id="d606b-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="d606b-107">Contatos</span><span class="sxs-lookup"><span data-stu-id="d606b-107">Contacts</span></span>                    | <span data-ttu-id="d606b-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d606b-108">Contacts.Read</span></span>       |
| <span data-ttu-id="d606b-109">Conversas</span><span class="sxs-lookup"><span data-stu-id="d606b-109">Conversations</span></span>               | <span data-ttu-id="d606b-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d606b-110">Group.Read.All</span></span>      |
| <span data-ttu-id="d606b-111">Eventos</span><span class="sxs-lookup"><span data-stu-id="d606b-111">Events</span></span>                      | <span data-ttu-id="d606b-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d606b-112">Calendars.Read</span></span>      |
| <span data-ttu-id="d606b-113">Mensagens</span><span class="sxs-lookup"><span data-stu-id="d606b-113">Messages</span></span>                    | <span data-ttu-id="d606b-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d606b-114">Mail.Read</span></span>           |
| <span data-ttu-id="d606b-115">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="d606b-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d606b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d606b-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d606b-117">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="d606b-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="d606b-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d606b-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d606b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d606b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d606b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d606b-120">Optional query parameters</span></span>
<span data-ttu-id="d606b-121">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d606b-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d606b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d606b-122">Request headers</span></span>
| <span data-ttu-id="d606b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d606b-123">Name</span></span>       | <span data-ttu-id="d606b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d606b-124">Type</span></span> | <span data-ttu-id="d606b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d606b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d606b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d606b-126">Authorization</span></span>  | <span data-ttu-id="d606b-127">string</span><span class="sxs-lookup"><span data-stu-id="d606b-127">string</span></span>  | <span data-ttu-id="d606b-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d606b-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d606b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d606b-130">Request body</span></span>
<span data-ttu-id="d606b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d606b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d606b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d606b-132">Response</span></span>

<span data-ttu-id="d606b-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d606b-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d606b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d606b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d606b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d606b-135">Request</span></span>
<span data-ttu-id="d606b-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d606b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="d606b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d606b-137">Response</span></span>
<span data-ttu-id="d606b-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d606b-138">Here is an example of the response.</span></span>
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

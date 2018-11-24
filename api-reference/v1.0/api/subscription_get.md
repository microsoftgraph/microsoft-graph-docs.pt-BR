# <a name="get-subscription"></a><span data-ttu-id="de0cc-101">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="de0cc-101">Get subscription</span></span>

<span data-ttu-id="de0cc-102">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="de0cc-102">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="de0cc-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="de0cc-103">Permissions</span></span>

<span data-ttu-id="de0cc-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="de0cc-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="de0cc-106">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="de0cc-106">Resource type / Item</span></span>        | <span data-ttu-id="de0cc-107">Permissão</span><span class="sxs-lookup"><span data-stu-id="de0cc-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="de0cc-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="de0cc-108">Contacts</span></span>                    | <span data-ttu-id="de0cc-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de0cc-109">Contacts.Read</span></span>       |
| <span data-ttu-id="de0cc-110">Conversas</span><span class="sxs-lookup"><span data-stu-id="de0cc-110">Conversations</span></span>               | <span data-ttu-id="de0cc-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="de0cc-111">Group.Read.All</span></span>      |
| <span data-ttu-id="de0cc-112">Eventos</span><span class="sxs-lookup"><span data-stu-id="de0cc-112">Events</span></span>                      | <span data-ttu-id="de0cc-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de0cc-113">Calendars.Read</span></span>      |
| <span data-ttu-id="de0cc-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="de0cc-114">Messages</span></span>                    | <span data-ttu-id="de0cc-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de0cc-115">Mail.Read</span></span>           |
| <span data-ttu-id="de0cc-116">Grupos</span><span class="sxs-lookup"><span data-stu-id="de0cc-116">Groups</span></span>                      | <span data-ttu-id="de0cc-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="de0cc-117">Group.Read.All</span></span>      |
| <span data-ttu-id="de0cc-118">Usuários</span><span class="sxs-lookup"><span data-stu-id="de0cc-118">Users</span></span>                       | <span data-ttu-id="de0cc-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="de0cc-119">User.Read.All</span></span>       |
| <span data-ttu-id="de0cc-120">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="de0cc-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="de0cc-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de0cc-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="de0cc-122">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="de0cc-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="de0cc-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de0cc-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="de0cc-124">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="de0cc-124">Security alert</span></span>| <span data-ttu-id="de0cc-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de0cc-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de0cc-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de0cc-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de0cc-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de0cc-127">Optional query parameters</span></span>

<span data-ttu-id="de0cc-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de0cc-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de0cc-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de0cc-129">Request headers</span></span>

| <span data-ttu-id="de0cc-130">Nome</span><span class="sxs-lookup"><span data-stu-id="de0cc-130">Name</span></span>       | <span data-ttu-id="de0cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="de0cc-131">Type</span></span> | <span data-ttu-id="de0cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="de0cc-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de0cc-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="de0cc-133">Authorization</span></span>  | <span data-ttu-id="de0cc-134">string</span><span class="sxs-lookup"><span data-stu-id="de0cc-134">string</span></span>  | <span data-ttu-id="de0cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de0cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de0cc-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de0cc-137">Request body</span></span>

<span data-ttu-id="de0cc-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de0cc-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de0cc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="de0cc-139">Response</span></span>

<span data-ttu-id="de0cc-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de0cc-140">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de0cc-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de0cc-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="de0cc-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de0cc-142">Request</span></span>

<span data-ttu-id="de0cc-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de0cc-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="de0cc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="de0cc-144">Response</span></span>

<span data-ttu-id="de0cc-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de0cc-145">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
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

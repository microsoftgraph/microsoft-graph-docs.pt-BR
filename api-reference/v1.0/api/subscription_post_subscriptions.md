# <a name="create-subscription"></a><span data-ttu-id="3ea23-101">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="3ea23-101">Create subscription</span></span>

<span data-ttu-id="3ea23-102">Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="3ea23-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ea23-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ea23-103">Permissions</span></span>

<span data-ttu-id="3ea23-p101">Criar uma assinatura exige escopo de leitura para o recurso. Por exemplo, para obter mensagens de notificações, seu aplicativo precisa da permissão `Mail.Read`. A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ea23-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="3ea23-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="3ea23-108">Resource type / Item</span></span>        | <span data-ttu-id="3ea23-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="3ea23-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="3ea23-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="3ea23-110">Contacts</span></span>                    | <span data-ttu-id="3ea23-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ea23-111">Contacts.Read</span></span>       |
| <span data-ttu-id="3ea23-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="3ea23-112">Conversations</span></span>               | <span data-ttu-id="3ea23-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea23-113">Group.Read.All</span></span>      |
| <span data-ttu-id="3ea23-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="3ea23-114">Events</span></span>                      | <span data-ttu-id="3ea23-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ea23-115">Calendars.Read</span></span>      |
| <span data-ttu-id="3ea23-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="3ea23-116">Messages</span></span>                    | <span data-ttu-id="3ea23-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ea23-117">Mail.Read</span></span>           |
| <span data-ttu-id="3ea23-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="3ea23-118">Groups</span></span>                      | <span data-ttu-id="3ea23-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea23-119">Group.Read.All</span></span>      |
| <span data-ttu-id="3ea23-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="3ea23-120">Users</span></span>                       | <span data-ttu-id="3ea23-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea23-121">User.Read.All</span></span>       |
| <span data-ttu-id="3ea23-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="3ea23-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="3ea23-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ea23-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="3ea23-124">Unidades (unidades e conteúdo compartilhado do SharePoint)</span><span class="sxs-lookup"><span data-stu-id="3ea23-124">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="3ea23-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea23-125">Files.ReadWrite.All</span></span> |

 > <span data-ttu-id="3ea23-126">**Observação:** O ponto de extremidade /v1.0 concede permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="3ea23-126">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="3ea23-127">Não há suporte para conversas em grupo e itens da unidade raiz do OneDrive com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea23-127">Note: The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ea23-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ea23-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="3ea23-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea23-129">Request headers</span></span>

| <span data-ttu-id="3ea23-130">Nome</span><span class="sxs-lookup"><span data-stu-id="3ea23-130">Name</span></span>       | <span data-ttu-id="3ea23-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ea23-131">Type</span></span> | <span data-ttu-id="3ea23-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ea23-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ea23-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ea23-133">Authorization</span></span>  | <span data-ttu-id="3ea23-134">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea23-134">string</span></span>  | <span data-ttu-id="3ea23-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ea23-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3ea23-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ea23-137">Response</span></span>

<span data-ttu-id="3ea23-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ea23-138">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ea23-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ea23-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ea23-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea23-140">Request</span></span>

<span data-ttu-id="3ea23-141">Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="3ea23-141">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="3ea23-142">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="3ea23-142">In the request body, supply a JSON representation of the [Contact](../resources/subscription.md) object.</span></span>
<span data-ttu-id="3ea23-143">O preenchimento do campo `clientState` é opcional.</span><span class="sxs-lookup"><span data-stu-id="3ea23-143">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="3ea23-144">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="3ea23-144">Resources examples</span></span>

<span data-ttu-id="3ea23-145">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="3ea23-145">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="3ea23-146">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="3ea23-146">Resource type</span></span> | <span data-ttu-id="3ea23-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ea23-147">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="3ea23-148">Email</span><span class="sxs-lookup"><span data-stu-id="3ea23-148">Mail</span></span>|<span data-ttu-id="3ea23-149">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="3ea23-149">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="3ea23-150">me/messages</span><span class="sxs-lookup"><span data-stu-id="3ea23-150">me/messages</span></span>|
|<span data-ttu-id="3ea23-151">Contatos</span><span class="sxs-lookup"><span data-stu-id="3ea23-151">Contacts</span></span>|<span data-ttu-id="3ea23-152">me/contacts</span><span class="sxs-lookup"><span data-stu-id="3ea23-152">me/contacts</span></span>|
|<span data-ttu-id="3ea23-153">Calendários</span><span class="sxs-lookup"><span data-stu-id="3ea23-153">Calendars</span></span>|<span data-ttu-id="3ea23-154">me/events</span><span class="sxs-lookup"><span data-stu-id="3ea23-154">me/events</span></span>|
|<span data-ttu-id="3ea23-155">Usuários</span><span class="sxs-lookup"><span data-stu-id="3ea23-155">Users</span></span>|<span data-ttu-id="3ea23-156">users</span><span class="sxs-lookup"><span data-stu-id="3ea23-156">users</span></span>|
|<span data-ttu-id="3ea23-157">Grupos</span><span class="sxs-lookup"><span data-stu-id="3ea23-157">Groups</span></span>|<span data-ttu-id="3ea23-158">groups</span><span class="sxs-lookup"><span data-stu-id="3ea23-158">Groups</span></span>|
|<span data-ttu-id="3ea23-159">Conversas</span><span class="sxs-lookup"><span data-stu-id="3ea23-159">Conversations</span></span>|<span data-ttu-id="3ea23-160">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="3ea23-160">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="3ea23-161">Unidades</span><span class="sxs-lookup"><span data-stu-id="3ea23-161">Drives</span></span>|<span data-ttu-id="3ea23-162">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="3ea23-162">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="3ea23-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ea23-163">Response</span></span>

<span data-ttu-id="3ea23-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ea23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="3ea23-167">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="3ea23-167">Notification endpoint validation</span></span>

<span data-ttu-id="3ea23-168">O ponto de extremidade de notificação de assinatura (especificado na propriedade `notificationUrl`) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](../../../concepts/webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="3ea23-168">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="3ea23-169">Se a validação falhar, a solicitação para criar a assinatura retornará um erro 400 de solicitação inválida.</span><span class="sxs-lookup"><span data-stu-id="3ea23-169">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

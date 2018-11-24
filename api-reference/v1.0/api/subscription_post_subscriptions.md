# <a name="create-subscription"></a><span data-ttu-id="85229-101">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="85229-101">Create subscription</span></span>

<span data-ttu-id="85229-102">Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="85229-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="85229-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="85229-103">Permissions</span></span>

<span data-ttu-id="85229-p101">Criar uma assinatura exige escopo de leitura para o recurso. Por exemplo, para obter mensagens de notificações, seu aplicativo precisa da permissão `Mail.Read`. A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="85229-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="85229-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="85229-108">Resource type / Item</span></span>        | <span data-ttu-id="85229-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="85229-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="85229-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="85229-110">Contacts</span></span>                    | <span data-ttu-id="85229-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="85229-111">Contacts.Read</span></span>       |
| <span data-ttu-id="85229-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="85229-112">Conversations</span></span>               | <span data-ttu-id="85229-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="85229-113">Group.Read.All</span></span>      |
| <span data-ttu-id="85229-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="85229-114">Events</span></span>                      | <span data-ttu-id="85229-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85229-115">Calendars.Read</span></span>      |
| <span data-ttu-id="85229-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="85229-116">Messages</span></span>                    | <span data-ttu-id="85229-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="85229-117">Mail.Read</span></span>           |
| <span data-ttu-id="85229-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="85229-118">Groups</span></span>                      | <span data-ttu-id="85229-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="85229-119">Group.Read.All</span></span>      |
| <span data-ttu-id="85229-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="85229-120">Users</span></span>                       | <span data-ttu-id="85229-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85229-121">User.Read.All</span></span>       |
| <span data-ttu-id="85229-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="85229-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="85229-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85229-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="85229-124">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="85229-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="85229-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85229-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="85229-126">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="85229-126">Security alert</span></span>| <span data-ttu-id="85229-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85229-127">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="85229-128">**Observação:** O ponto de extremidade /v1.0 permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="85229-128">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="85229-129">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85229-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="85229-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85229-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="85229-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85229-131">Request headers</span></span>

| <span data-ttu-id="85229-132">Nome</span><span class="sxs-lookup"><span data-stu-id="85229-132">Name</span></span>       | <span data-ttu-id="85229-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="85229-133">Type</span></span> | <span data-ttu-id="85229-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="85229-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="85229-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="85229-135">Authorization</span></span>  | <span data-ttu-id="85229-136">string</span><span class="sxs-lookup"><span data-stu-id="85229-136">string</span></span>  | <span data-ttu-id="85229-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85229-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="85229-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="85229-139">Response</span></span>

<span data-ttu-id="85229-140">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85229-140">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85229-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85229-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85229-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85229-142">Request</span></span>

<span data-ttu-id="85229-143">Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="85229-143">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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

<span data-ttu-id="85229-144">No corpo da solicitação, fornece uma representação JSON do objeto de [inscrição](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="85229-144">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="85229-145">O `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="85229-145">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="85229-146">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="85229-146">Resources examples</span></span>

<span data-ttu-id="85229-147">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="85229-147">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="85229-148">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="85229-148">Resource type</span></span> | <span data-ttu-id="85229-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85229-149">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="85229-150">Email</span><span class="sxs-lookup"><span data-stu-id="85229-150">Mail</span></span>|<span data-ttu-id="85229-151">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="85229-151">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="85229-152">me/messages</span><span class="sxs-lookup"><span data-stu-id="85229-152">me/messages</span></span>|
|<span data-ttu-id="85229-153">Contatos</span><span class="sxs-lookup"><span data-stu-id="85229-153">Contacts</span></span>|<span data-ttu-id="85229-154">me/contacts</span><span class="sxs-lookup"><span data-stu-id="85229-154">me/contacts</span></span>|
|<span data-ttu-id="85229-155">Calendários</span><span class="sxs-lookup"><span data-stu-id="85229-155">Calendars</span></span>|<span data-ttu-id="85229-156">me/events</span><span class="sxs-lookup"><span data-stu-id="85229-156">me/events</span></span>|
|<span data-ttu-id="85229-157">Usuários</span><span class="sxs-lookup"><span data-stu-id="85229-157">Users</span></span>|<span data-ttu-id="85229-158">users</span><span class="sxs-lookup"><span data-stu-id="85229-158">users</span></span>|
|<span data-ttu-id="85229-159">Grupos</span><span class="sxs-lookup"><span data-stu-id="85229-159">Groups</span></span>|<span data-ttu-id="85229-160">grupos</span><span class="sxs-lookup"><span data-stu-id="85229-160">groups</span></span>|
|<span data-ttu-id="85229-161">Conversas</span><span class="sxs-lookup"><span data-stu-id="85229-161">Conversations</span></span>|<span data-ttu-id="85229-162">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="85229-162">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="85229-163">Unidades</span><span class="sxs-lookup"><span data-stu-id="85229-163">Drives</span></span>|<span data-ttu-id="85229-164">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="85229-164">me/drive/root</span></span>|
|<span data-ttu-id="85229-165">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="85229-165">Security alert</span></span>|<span data-ttu-id="85229-166">alertas de segurança /? $filter = status eq 'Novo'</span><span class="sxs-lookup"><span data-stu-id="85229-166">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="85229-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="85229-167">Response</span></span>

<span data-ttu-id="85229-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85229-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="85229-171">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="85229-171">Notification endpoint validation</span></span>

<span data-ttu-id="85229-172">O ponto de extremidade de notificação de inscrição (especificado no `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para que as alterações nos dados do usuário](../../../concepts/webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="85229-172">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="85229-173">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de solicitação inválida a 400.</span><span class="sxs-lookup"><span data-stu-id="85229-173">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

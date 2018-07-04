# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="f0933-101">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="f0933-101">Set up notifications for changes in user data</span></span>

<span data-ttu-id="f0933-p101">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="f0933-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="f0933-105">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-105">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span> <span data-ttu-id="f0933-106">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="f0933-106">The app then takes action according to its business logic.</span></span> <span data-ttu-id="f0933-107">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="f0933-107">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="f0933-108">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="f0933-108">Supported resources</span></span>

<span data-ttu-id="f0933-109">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="f0933-109">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="f0933-110">Mensagens</span><span class="sxs-lookup"><span data-stu-id="f0933-110">Messages</span></span>
- <span data-ttu-id="f0933-111">Eventos</span><span class="sxs-lookup"><span data-stu-id="f0933-111">Events</span></span>
- <span data-ttu-id="f0933-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="f0933-112">Contacts</span></span>
- <span data-ttu-id="f0933-113">Usuários</span><span class="sxs-lookup"><span data-stu-id="f0933-113">Users</span></span>
- <span data-ttu-id="f0933-114">Grupos</span><span class="sxs-lookup"><span data-stu-id="f0933-114">Groups</span></span>
- <span data-ttu-id="f0933-115">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="f0933-115">Group conversations</span></span>
- <span data-ttu-id="f0933-116">Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="f0933-116">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="f0933-117">Pastas de OneDrive pessoais do usuário</span><span class="sxs-lookup"><span data-stu-id="f0933-117">User's personal OneDrive folders</span></span>

<span data-ttu-id="f0933-118">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="f0933-118">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="f0933-119">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="f0933-119">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="f0933-120">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="f0933-120">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="f0933-121">Ou para uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="f0933-121">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="f0933-122">Ou para o OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="f0933-122">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="f0933-123">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="f0933-123">Azure AD Resource Limitations</span></span>

<span data-ttu-id="f0933-124">Determinados limites se aplicam aos recursos baseados no Microsoft Azure AD (usuários, grupos) e podem gerar erros quando excedidos:</span><span class="sxs-lookup"><span data-stu-id="f0933-124">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="f0933-125">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="f0933-125">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="f0933-126">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="f0933-126">Per App: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="f0933-127">Por locatário: total de 35 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="f0933-127">Per Tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="f0933-128">Combinação por aplicativo e locatário: sete assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="f0933-128">Per App and Tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="f0933-129">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="f0933-129">Azure AD B2C tenants are not supported</span></span>

- <span data-ttu-id="f0933-130">Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="f0933-130">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="f0933-131">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-131">Subscription lifetime</span></span>

<span data-ttu-id="f0933-132">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="f0933-132">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="f0933-133">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="f0933-133">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="f0933-134">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-134">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="f0933-135">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="f0933-135">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="f0933-136">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="f0933-136">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="f0933-137">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="f0933-137">Managing subscriptions</span></span>

<span data-ttu-id="f0933-138">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="f0933-138">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="f0933-139">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-139">Creating a subscription</span></span>

<span data-ttu-id="f0933-p104">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="f0933-p104">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="f0933-142">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="f0933-142">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="f0933-143">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0933-143">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="f0933-144">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="f0933-144">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="f0933-145">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="f0933-145">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="f0933-146">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f0933-146">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="f0933-147">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="f0933-147">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="f0933-148">O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="f0933-149">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-149">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="f0933-150">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="f0933-150">The `changeType`, `notificationUrl`, `resource` and `expirationDateTime` properties are required while the rest are optional.</span></span> <span data-ttu-id="f0933-151">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](../api-reference/v1.0/resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="f0933-151">See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values.</span></span>

<span data-ttu-id="f0933-152">Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="f0933-152">The , , , and  properties are required. See subscription resource type for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="f0933-153">A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f0933-153">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="f0933-154">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f0933-154">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="f0933-155">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](../api-reference/v1.0/resources/subscription.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="f0933-155">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="f0933-156">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="f0933-156">Notification endpoint validation</span></span>

<span data-ttu-id="f0933-157">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-157">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="f0933-158">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="f0933-158">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="f0933-159">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="f0933-159">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ```

1. <span data-ttu-id="f0933-160">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="f0933-160">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="f0933-161">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="f0933-161">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="f0933-162">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="f0933-162">The content type must be text/plain.</span></span>
    - <span data-ttu-id="f0933-163">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f0933-163">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="f0933-164">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="f0933-164">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="f0933-165">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-165">Renewing a subscription</span></span>

<span data-ttu-id="f0933-166">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0933-166">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span> <span data-ttu-id="f0933-167">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f0933-167">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="f0933-168">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-168">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="f0933-169">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](../api-reference/v1.0/resources/subscription.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="f0933-169">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span> <span data-ttu-id="f0933-170">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="f0933-170">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="f0933-171">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-171">Deleting a subscription</span></span>

<span data-ttu-id="f0933-172">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="f0933-172">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="f0933-173">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f0933-173">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="f0933-174">Notificações</span><span class="sxs-lookup"><span data-stu-id="f0933-174">Notifications</span></span>

<span data-ttu-id="f0933-175">O cliente começa a receber notificações depois de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-175">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="f0933-176">O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="f0933-176">Microsoft Graph sends a POST request to the notification URL:</span></span> <span data-ttu-id="f0933-177">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="f0933-177">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="f0933-178">**Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes.</span><span class="sxs-lookup"><span data-stu-id="f0933-178">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="f0933-179">Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-179">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="f0933-180">Propriedades do objeto notification</span><span class="sxs-lookup"><span data-stu-id="f0933-180">Notification properties</span></span>

<span data-ttu-id="f0933-181">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="f0933-181">The notification object has the following properties:</span></span>

| <span data-ttu-id="f0933-182">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0933-182">Property</span></span> | <span data-ttu-id="f0933-183">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0933-183">Type</span></span> | <span data-ttu-id="f0933-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0933-184">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f0933-185">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="f0933-185">subscriptionId</span></span> | <span data-ttu-id="f0933-186">string</span><span class="sxs-lookup"><span data-stu-id="f0933-186">string</span></span> | <span data-ttu-id="f0933-187">A ID da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="f0933-187">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="f0933-188">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f0933-188">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="f0933-189">dateTime</span><span class="sxs-lookup"><span data-stu-id="f0933-189">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="f0933-190">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-190">: The expiration time for the subscription.</span></span> |
| <span data-ttu-id="f0933-191">clientState</span><span class="sxs-lookup"><span data-stu-id="f0933-191">clientState</span></span> | <span data-ttu-id="f0933-192">string</span><span class="sxs-lookup"><span data-stu-id="f0933-192">string</span></span> | <span data-ttu-id="f0933-193">A propriedade `clientState` especificada na solicitação de assinatura. (caso haja).</span><span class="sxs-lookup"><span data-stu-id="f0933-193">clientState - The clientState property specified in the subscription request.</span></span> |
| <span data-ttu-id="f0933-194">changeType</span><span class="sxs-lookup"><span data-stu-id="f0933-194">changeType</span></span> | <span data-ttu-id="f0933-195">string</span><span class="sxs-lookup"><span data-stu-id="f0933-195">string</span></span> | <span data-ttu-id="f0933-196">O tipo de evento que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="f0933-196">The event type that caused the notification.</span></span> <span data-ttu-id="f0933-197">Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="f0933-197">changeType - The event type that caused the notification. For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="f0933-198">recurso</span><span class="sxs-lookup"><span data-stu-id="f0933-198">resource</span></span> | <span data-ttu-id="f0933-199">string</span><span class="sxs-lookup"><span data-stu-id="f0933-199">string</span></span> | <span data-ttu-id="f0933-200">O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="f0933-200">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="f0933-201">resourceData</span><span class="sxs-lookup"><span data-stu-id="f0933-201">ResourceData</span></span> | <span data-ttu-id="f0933-202">objeto</span><span class="sxs-lookup"><span data-stu-id="f0933-202">object</span></span> | <span data-ttu-id="f0933-203">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="f0933-203">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="f0933-204">Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="f0933-204">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="f0933-205">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0933-205">Property</span></span> | <span data-ttu-id="f0933-206">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0933-206">Type</span></span> | <span data-ttu-id="f0933-207">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0933-207">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f0933-208">@odata.type</span><span class="sxs-lookup"><span data-stu-id="f0933-208">@odata.type</span></span> | <span data-ttu-id="f0933-209">string</span><span class="sxs-lookup"><span data-stu-id="f0933-209">string</span></span> | <span data-ttu-id="f0933-210">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="f0933-210">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="f0933-211">@odata.id</span><span class="sxs-lookup"><span data-stu-id="f0933-211">@odata.id</span></span> | <span data-ttu-id="f0933-212">string</span><span class="sxs-lookup"><span data-stu-id="f0933-212">string</span></span> | <span data-ttu-id="f0933-213">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0933-213">@odata.id - The OData identifier of the object.</span></span> |
| <span data-ttu-id="f0933-214">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="f0933-214">@odata.etag</span></span> | <span data-ttu-id="f0933-215">string</span><span class="sxs-lookup"><span data-stu-id="f0933-215">string</span></span> | <span data-ttu-id="f0933-216">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0933-216">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span> |
| <span data-ttu-id="f0933-217">id</span><span class="sxs-lookup"><span data-stu-id="f0933-217">id</span></span> | <span data-ttu-id="f0933-218">string</span><span class="sxs-lookup"><span data-stu-id="f0933-218">string</span></span> | <span data-ttu-id="f0933-219">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0933-219">Id - The identifier of the object.</span></span> |

> <span data-ttu-id="f0933-220">**Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada.</span><span class="sxs-lookup"><span data-stu-id="f0933-220">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="f0933-221">Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.</span><span class="sxs-lookup"><span data-stu-id="f0933-221">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="f0933-222">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="f0933-222">Notification example</span></span>

<span data-ttu-id="f0933-223">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="f0933-223">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

<span data-ttu-id="f0933-224">Observe que o campo `value` é uma matriz de objetos.</span><span class="sxs-lookup"><span data-stu-id="f0933-224">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="f0933-225">Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0933-225">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="f0933-226">Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.</span><span class="sxs-lookup"><span data-stu-id="f0933-226">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="f0933-227">Processar a notificação</span><span class="sxs-lookup"><span data-stu-id="f0933-227">Processing the notification</span></span>

<span data-ttu-id="f0933-228">Cada notificação recebida por seu aplicativo deve ser processada.</span><span class="sxs-lookup"><span data-stu-id="f0933-228">Each notification received by your app should be processed.</span></span> <span data-ttu-id="f0933-229">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="f0933-229">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="f0933-230">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="f0933-230">Validate the `clientState` property.</span></span> <span data-ttu-id="f0933-231">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-231">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="f0933-232">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="f0933-232">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="f0933-233">É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="f0933-233">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="f0933-234">Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="f0933-234">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="f0933-235">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="f0933-235">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="f0933-236">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f0933-236">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="f0933-237">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.</span><span class="sxs-lookup"><span data-stu-id="f0933-237">Send a  status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>

    > <span data-ttu-id="f0933-238">**Observação:** você deve enviar um código de status `202 - Accepted` mesmo que a propriedade `clientState` não corresponda àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="f0933-238">You should send a  status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="f0933-239">Essa é uma boa prática, uma vez que impede que um possível ator invasor descubra que você não confia nas notificações dele e use as informações para tentar adivinhar o valor da propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="f0933-239">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="f0933-240">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0933-240">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="f0933-241">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="f0933-241">Code samples</span></span>

<span data-ttu-id="f0933-242">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="f0933-242">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="f0933-243">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="f0933-243">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="f0933-244">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="f0933-244">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="f0933-245">Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs</span><span class="sxs-lookup"><span data-stu-id="f0933-245">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="f0933-246">Confira também</span><span class="sxs-lookup"><span data-stu-id="f0933-246">See also</span></span>

- [<span data-ttu-id="f0933-247">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-247">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
- [<span data-ttu-id="f0933-248">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-248">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
- [<span data-ttu-id="f0933-249">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="f0933-249">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)

[contact]: ../api-reference/v1.0/resources/contact.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[drive]: ../api-reference/v1.0/resources/drive.md
[event]: ../api-reference/v1.0/resources/event.md
[message]: ../api-reference/v1.0/resources/message.md

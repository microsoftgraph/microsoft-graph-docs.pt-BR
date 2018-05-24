# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="0e87e-101">Trabalhando com webhooks no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e87e-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="0e87e-p101">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="0e87e-105">Usando a API REST do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="0e87e-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="0e87e-106">Mensagens</span><span class="sxs-lookup"><span data-stu-id="0e87e-106">Messages</span></span>
* <span data-ttu-id="0e87e-107">Eventos</span><span class="sxs-lookup"><span data-stu-id="0e87e-107">Events</span></span>
* <span data-ttu-id="0e87e-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="0e87e-108">Contacts</span></span>
* <span data-ttu-id="0e87e-109">Usuários</span><span class="sxs-lookup"><span data-stu-id="0e87e-109">Users</span></span>
* <span data-ttu-id="0e87e-110">Grupos</span><span class="sxs-lookup"><span data-stu-id="0e87e-110">Groups</span></span>
* <span data-ttu-id="0e87e-111">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="0e87e-111">Group conversations</span></span>
* <span data-ttu-id="0e87e-112">Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e87e-112">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="0e87e-113">Pastas de OneDrive pessoais do usuário</span><span class="sxs-lookup"><span data-stu-id="0e87e-113">User's personal OneDrive folders</span></span>

<span data-ttu-id="0e87e-114">Por exemplo, você pode criar uma assinatura para uma pasta específica: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="0e87e-114">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="0e87e-115">Ou uma ID específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="0e87e-115">Or a specific ID: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="0e87e-116">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="0e87e-116">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`</span></span>

<span data-ttu-id="0e87e-117">Ou em uma unidade do Sharepoint / OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="0e87e-117">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="0e87e-118">Ou no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="0e87e-118">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="0e87e-p102">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura. O aplicativo então realiza ações de acordo com sua lógica comercial. Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="0e87e-122">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="0e87e-122">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="0e87e-123">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="0e87e-123">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="0e87e-124">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="0e87e-124">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="0e87e-125">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="0e87e-125">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="0e87e-p104">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api-reference/v1.0/api/subscription_post_subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api-reference/v1.0/api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="0e87e-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e87e-130">Permission type</span></span>                        | <span data-ttu-id="0e87e-131">Tipos de recurso com suporte na v1.0</span><span class="sxs-lookup"><span data-stu-id="0e87e-131">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="0e87e-132">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="0e87e-132">Delegated - work or school account</span></span>     | <span data-ttu-id="0e87e-133">[contact][], [conversation][], [drive][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="0e87e-133">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="0e87e-134">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="0e87e-134">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="0e87e-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e87e-135">None</span></span>                                                             |
| <span data-ttu-id="0e87e-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e87e-136">Application</span></span>                            | <span data-ttu-id="0e87e-137">[contact][], [conversation][], [event][], [message][]</span><span class="sxs-lookup"><span data-stu-id="0e87e-137">[contact][], [conversation][], [event][], [message][]</span></span>            |


## <a name="code-samples"></a><span data-ttu-id="0e87e-138">Code samples</span><span class="sxs-lookup"><span data-stu-id="0e87e-138">Code samples</span></span>

<span data-ttu-id="0e87e-139">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="0e87e-139">The following code samples are available on GitHub.</span></span>

* [<span data-ttu-id="0e87e-140">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="0e87e-140">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="0e87e-141">Exemplo de webhooks do Microsoft Graph para ASP,NET</span><span class="sxs-lookup"><span data-stu-id="0e87e-141">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

### <a name="creating-a-subscription"></a><span data-ttu-id="0e87e-142">Criando uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-142">Creating a subscription</span></span>

<span data-ttu-id="0e87e-p105">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="0e87e-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="0e87e-145">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="0e87e-145">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="0e87e-146">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e87e-146">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="0e87e-147">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="0e87e-147">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="0e87e-148">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="0e87e-148">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="0e87e-149">O cliente enviará o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0e87e-149">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="0e87e-150">O cliente deve armazenar a ID da assinatura para correlacionar uma notificação com a assinatura correspondente.</span><span class="sxs-lookup"><span data-stu-id="0e87e-150">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

### <a name="notification-url-validation"></a><span data-ttu-id="0e87e-151">Validação da URL de notificação</span><span class="sxs-lookup"><span data-stu-id="0e87e-151">Notification URL validation</span></span>

<span data-ttu-id="0e87e-p106">O Microsoft Graph valida a URL de notificação em uma solicitação de assinatura antes de criar a assinatura. O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="0e87e-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="0e87e-154">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="0e87e-154">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```

2. <span data-ttu-id="0e87e-155">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="0e87e-155">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="0e87e-156">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="0e87e-156">A 200 (OK) status code.</span></span>
  * <span data-ttu-id="0e87e-157">O tipo de conteúdo deve ser texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="0e87e-157">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="0e87e-158">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0e87e-158">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="0e87e-159">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="0e87e-159">The client should discard the validation token after providing it in the response.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="0e87e-160">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-160">Subscription request example</span></span>

``` http
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

<span data-ttu-id="0e87e-p107">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias. Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](../api-reference/v1.0/resources/subscription.md). Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="0e87e-164">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](../api-reference/v1.0/resources/subscription.md) no corpo. </span><span class="sxs-lookup"><span data-stu-id="0e87e-164">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="0e87e-165">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="0e87e-165">Azure AD Resource Limitations</span></span>

<span data-ttu-id="0e87e-166">Determinados limites se aplicam aos recursos baseados no Microsoft Azure AD (usuários, grupos) e podem gerar erros quando excedidos:</span><span class="sxs-lookup"><span data-stu-id="0e87e-166">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

* <span data-ttu-id="0e87e-167">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="0e87e-167">Maximum subscription quotas:</span></span>

  * <span data-ttu-id="0e87e-168">Por aplicativo: total de 50.000 assinaturas</span><span class="sxs-lookup"><span data-stu-id="0e87e-168">Per App: 50,000 total subscriptions</span></span>
  * <span data-ttu-id="0e87e-169">Por locatário: total de 35 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="0e87e-169">Per Tenant: 35 total subscriptions across all apps</span></span>
  * <span data-ttu-id="0e87e-170">Por combinação de aplicativo e locatário: 7 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="0e87e-170">Per App and Tenant combination: 7 total subscriptions</span></span>

* <span data-ttu-id="0e87e-171">Os locatários do Microsoft Azure AD B2C não são suportados</span><span class="sxs-lookup"><span data-stu-id="0e87e-171">Azure AD B2C tenants are not supported</span></span>

* <span data-ttu-id="0e87e-172">Usuários da conta do consumidor não são suportados</span><span class="sxs-lookup"><span data-stu-id="0e87e-172">Consumer account Users not supported</span></span>

## <a name="renewing-a-subscription"></a><span data-ttu-id="0e87e-173">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-173">Renewing a subscription</span></span>

<span data-ttu-id="0e87e-p108">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação. A propriedade expirationDateTime é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

### <a name="subscription-renewal-example"></a><span data-ttu-id="0e87e-176">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-176">Subscription renewal example</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="0e87e-p109">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](../api-reference/v1.0/resources/subscription.md) no corpo. O objeto subscription inclui o novo valor de expirationDateTime.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

## <a name="deleting-a-subscription"></a><span data-ttu-id="0e87e-179">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-179">Deleting a subscription</span></span>

<span data-ttu-id="0e87e-180">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="0e87e-180">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="0e87e-181">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e87e-181">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="0e87e-182">Notificações</span><span class="sxs-lookup"><span data-stu-id="0e87e-182">Notifications</span></span>

<span data-ttu-id="0e87e-p110">O cliente começa a receber notificações depois de criar a assinatura. O Microsoft Graph envia uma solicitação POST à URL de notificação quando ocorrem alterações no recurso. O cliente só recebe notificações de acordo com o tipo de alteração especificada, como *created*.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="0e87e-186">Propriedades de notification</span><span class="sxs-lookup"><span data-stu-id="0e87e-186">Notification properties</span></span>

<span data-ttu-id="0e87e-187">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="0e87e-187">The notification object has the following properties:</span></span>

* <span data-ttu-id="0e87e-188">subscriptionId – A ID da assinatura à qual essa notificação pertence.</span><span class="sxs-lookup"><span data-stu-id="0e87e-188">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="0e87e-189">subscriptionExpirationDateTime – O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0e87e-189">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="0e87e-190">clientState – A propriedade clientState especificada na solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="0e87e-190">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="0e87e-p111">changeType – O tipo de evento que gerou a notificação. Por exemplo, *created* ao receber um email ou *updated* ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="0e87e-193">resource – O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="0e87e-193">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="0e87e-p112">resourceData – O objeto dependente do recurso que está sendo assinado.  Por exemplo, para recursos do Outlook:</span><span class="sxs-lookup"><span data-stu-id="0e87e-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="0e87e-196">@odata.type – O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="0e87e-196">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="0e87e-197">@odata.id – O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="0e87e-197">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="0e87e-198">@odata.etag – A marca da entidade HTTP que representa uma versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="0e87e-198">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="0e87e-199">id – O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="0e87e-199">id - The identifier of the object.</span></span>

> <span data-ttu-id="0e87e-p113">Observação: o valor de Id fornecido em resourceData é válido no momento em que a notificação é enfileirada. Algumas ações, como mover uma mensagem para outra pasta, podem resultar na alteração da Id de um recurso.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

### <a name="notification-example"></a><span data-ttu-id="0e87e-202">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="0e87e-202">Notification example</span></span>

<span data-ttu-id="0e87e-203">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="0e87e-203">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

``` json
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
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

<span data-ttu-id="0e87e-p114">Observe que o objeto value contém uma lista. Se houver muitas notificações na fila, o Microsoft Graph as enviará em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p114">Note the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="0e87e-206">Processando a notificação</span><span class="sxs-lookup"><span data-stu-id="0e87e-206">Processing the notification</span></span>

<span data-ttu-id="0e87e-p115">Depois que o seu aplicativo começar a receber notificações, ele precisa processá-las. Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="0e87e-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="0e87e-p116">Validar a propriedade `clientState`. A propriedade clientState na notificação deve corresponder àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="0e87e-p117">Observação: se isso não for verdadeiro, você não deve considerá-la uma notificação válida. Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="0e87e-213">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="0e87e-213">Update your application based on your business logic.</span></span>

3. <span data-ttu-id="0e87e-p118">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.</span><span class="sxs-lookup"><span data-stu-id="0e87e-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="0e87e-216">Você deve enviar um código de status `202 - Accepted` mesmo que a propriedade clientState não corresponda àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="0e87e-216">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="0e87e-217">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e87e-217">Repeat for other notifications in the request.</span></span>

## <a name="see-also"></a><span data-ttu-id="0e87e-218">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e87e-218">See also</span></span>

* [<span data-ttu-id="0e87e-219">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-219">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
* [<span data-ttu-id="0e87e-220">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-220">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
* [<span data-ttu-id="0e87e-221">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="0e87e-221">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)
* [<span data-ttu-id="0e87e-222">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="0e87e-222">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="0e87e-223">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="0e87e-223">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

[contato]: ../api-reference/v1.0/resources/contact.md
[contact]: ../api-reference/v1.0/resources/contact.md
[conversa]: ../api-reference/v1.0/resources/conversation.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[unidade]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
[evento]: ../api-reference/v1.0/resources/event.md
[event]: ../api-reference/v1.0/resources/event.md
[mensagem]: ../api-reference/v1.0/resources/message.md
[message]: ../api-reference/v1.0/resources/message.md

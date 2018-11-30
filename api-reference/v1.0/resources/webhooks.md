# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="2e974-101">Trabalhando com webhooks no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e974-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="2e974-p101">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="2e974-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="2e974-105">Usando a API REST do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="2e974-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="2e974-106">Mensagens</span><span class="sxs-lookup"><span data-stu-id="2e974-106">Messages</span></span>
* <span data-ttu-id="2e974-107">Eventos</span><span class="sxs-lookup"><span data-stu-id="2e974-107">Events</span></span>
* <span data-ttu-id="2e974-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="2e974-108">Contacts</span></span>
* <span data-ttu-id="2e974-109">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="2e974-109">Group conversations</span></span>
* <span data-ttu-id="2e974-110">Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="2e974-110">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="2e974-111">Pastas de OneDrive pessoais do usuário</span><span class="sxs-lookup"><span data-stu-id="2e974-111">User's personal OneDrive folders</span></span>

<span data-ttu-id="2e974-112">Por exemplo, você pode criar uma assinatura para uma pasta específica: `me/mailfolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="2e974-112">You can create a subscription to a specific folder: `me/mailfolders('inbox')/messages`</span></span>

<span data-ttu-id="2e974-113">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`</span><span class="sxs-lookup"><span data-stu-id="2e974-113">Or to a top-level resource: `me/messages`</span></span>

<span data-ttu-id="2e974-114">Ou em uma unidade do Sharepoint / OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="2e974-114">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="2e974-115">Ou no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="2e974-115">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="2e974-p102">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura. O aplicativo então realiza ações de acordo com sua lógica comercial. Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="2e974-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="2e974-p103">Os aplicativos devem renovar suas assinaturas antes de expirarem. Atualmente, o tempo de expiração mais longo é de três dias menos 90 minutos do tempo de criação. Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração. Caso contrário, eles precisarão criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="2e974-p103">Subscriptions expire. The current longest expiration time is three days minus 90 minutes (4230 in total) from the time of creation. Apps need to renew their subscriptions before the expiration time. Otherwise they'll need to create a new subscription.</span></span>

<span data-ttu-id="2e974-123">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="2e974-123">Apps should renew their subscriptions before they expire. They can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="2e974-p104">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription_post_subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="2e974-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="2e974-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e974-128">Permission type</span></span> | <span data-ttu-id="2e974-129">Tipos de recurso com suporte na v1.0</span><span class="sxs-lookup"><span data-stu-id="2e974-129">Supported resource types in v1.0</span></span> |
|:----------------|:---------------------------------|
| <span data-ttu-id="2e974-130">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="2e974-130">Delegated - work or school account</span></span> | [<span data-ttu-id="2e974-131">contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message</span><span class="sxs-lookup"><span data-stu-id="2e974-131">contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message</span></span>](message.md) |
| <span data-ttu-id="2e974-132">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2e974-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="2e974-133">None</span><span class="sxs-lookup"><span data-stu-id="2e974-133">None</span></span> |
| <span data-ttu-id="2e974-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e974-134">Application</span></span> | [<span data-ttu-id="2e974-135">contact](contact.md), [conversation](conversation.md), [event](event.md), [message</span><span class="sxs-lookup"><span data-stu-id="2e974-135">contact](contact.md), [conversation](conversation.md), [event](event.md), [message</span></span>](message.md) |

## <a name="code-samples"></a><span data-ttu-id="2e974-136">Code samples</span><span class="sxs-lookup"><span data-stu-id="2e974-136">Code samples</span></span>

<span data-ttu-id="2e974-137">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="2e974-137">The following samples are available on GitHub in the OneDrive organization.</span></span>

* [<span data-ttu-id="2e974-138">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="2e974-138">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="2e974-139">Exemplo de webhooks do Microsoft Graph para ASP,NET</span><span class="sxs-lookup"><span data-stu-id="2e974-139">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

# <a name="creating-a-subscription"></a><span data-ttu-id="2e974-140">Criando uma assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-140">Creating a subscription</span></span>

<span data-ttu-id="2e974-p105">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2e974-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="2e974-143">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="2e974-143">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="2e974-144">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e974-144">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="2e974-145">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="2e974-145">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="2e974-146">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="2e974-146">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="2e974-147">O cliente enviará o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2e974-147">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="2e974-148">O cliente deve armazenar a ID da assinatura para correlacionar uma notificação com a assinatura correspondente.</span><span class="sxs-lookup"><span data-stu-id="2e974-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

## <a name="notification-url-validation"></a><span data-ttu-id="2e974-149">Validação da URL de notificação</span><span class="sxs-lookup"><span data-stu-id="2e974-149">Notification URL validation</span></span>

<span data-ttu-id="2e974-p106">O Microsoft Graph valida a URL de notificação em uma solicitação de assinatura antes de criar a assinatura. O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2e974-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="2e974-152">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="2e974-152">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. <span data-ttu-id="2e974-153">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="2e974-153">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="2e974-154">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="2e974-154">An 200 (OK) status code.</span></span>
  * <span data-ttu-id="2e974-155">O tipo de conteúdo deve ser texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="2e974-155">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="2e974-156">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2e974-156">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="2e974-157">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="2e974-157">The client should discard the validation token after providing it in the response.</span></span>

## <a name="subscription-request-example"></a><span data-ttu-id="2e974-158">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-158">Subscription request example</span></span>

```
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

<span data-ttu-id="2e974-p107">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias. Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](subscription.md). Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="2e974-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="2e974-162">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](subscription.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="2e974-162">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](subscription.md) object in the body.</span></span>

# <a name="renewing-a-subscription"></a><span data-ttu-id="2e974-163">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-163">Renewing a subscription</span></span>

<span data-ttu-id="2e974-p108">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação. A propriedade expirationDateTime é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="2e974-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

## <a name="subscription-renewal-example"></a><span data-ttu-id="2e974-166">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-166">Subscription renewal example</span></span>

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="2e974-p109">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](subscription.md) no corpo. O objeto subscription inclui o novo valor de expirationDateTime.</span><span class="sxs-lookup"><span data-stu-id="2e974-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

# <a name="deleting-a-subscription"></a><span data-ttu-id="2e974-169">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-169">Deleting a subscription</span></span>

<span data-ttu-id="2e974-170">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="2e974-170">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="2e974-171">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2e974-171">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

# <a name="notifications"></a><span data-ttu-id="2e974-172">Notificações</span><span class="sxs-lookup"><span data-stu-id="2e974-172">Notifications</span></span>

<span data-ttu-id="2e974-p110">O cliente começa a receber notificações depois de criar a assinatura. O Microsoft Graph envia uma solicitação POST à URL de notificação quando ocorrem alterações no recurso. O cliente só recebe notificações de acordo com o tipo de alteração especificada, como *created*.</span><span class="sxs-lookup"><span data-stu-id="2e974-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

## <a name="notification-properties"></a><span data-ttu-id="2e974-176">Propriedades de notification</span><span class="sxs-lookup"><span data-stu-id="2e974-176">Notification properties</span></span>

<span data-ttu-id="2e974-177">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="2e974-177">The notification object has the following properties:</span></span>

* <span data-ttu-id="2e974-178">subscriptionId – A ID da assinatura à qual essa notificação pertence.</span><span class="sxs-lookup"><span data-stu-id="2e974-178">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="2e974-179">subscriptionExpirationDateTime – O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="2e974-179">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="2e974-180">clientState – A propriedade clientState especificada na solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="2e974-180">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="2e974-p111">changeType – O tipo de evento que gerou a notificação. Por exemplo, *created* ao receber um email ou *updated* ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="2e974-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="2e974-183">resource – O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="2e974-183">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="2e974-p112">resourceData – O objeto dependente do recurso que está sendo assinado.  Por exemplo, para recursos do Outlook:</span><span class="sxs-lookup"><span data-stu-id="2e974-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="2e974-186">@odata.type – O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="2e974-186">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="2e974-187">@odata.id – O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="2e974-187">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="2e974-188">@odata.etag – A marca da entidade HTTP que representa uma versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="2e974-188">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="2e974-189">id – O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="2e974-189">id - The identifier of the object.</span></span>


> <span data-ttu-id="2e974-p113">Observação: O valor de Id fornecido em resourceData é válido no momento em que a notificação é enfileirada. Algumas ações, como mover uma mensagem para outra pasta, podem resultar na alteração da Id de um recurso.</span><span class="sxs-lookup"><span data-stu-id="2e974-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

## <a name="notification-example"></a><span data-ttu-id="2e974-192">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="2e974-192">Notification example</span></span>

<span data-ttu-id="2e974-193">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="2e974-193">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```
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

<span data-ttu-id="2e974-p114">Observe que o objeto value contém uma lista. Se houver muitas notificações na fila, o Microsoft Graph as enviará em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e974-p114">Note that the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

## <a name="processing-the-notification"></a><span data-ttu-id="2e974-196">Processando a notificação</span><span class="sxs-lookup"><span data-stu-id="2e974-196">Processing the notification</span></span>

<span data-ttu-id="2e974-p115">Depois que o seu aplicativo começar a receber notificações, ele precisa processá-las. Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="2e974-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="2e974-p116">Validar a propriedade `clientState`. A propriedade clientState na notificação deve corresponder àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="2e974-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="2e974-p117">Observação: Se isso não for verdadeiro, você não deve considerá-la uma notificação válida. Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="2e974-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="2e974-203">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="2e974-203">Update your application based on your business logic.</span></span>
3. <span data-ttu-id="2e974-p118">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.</span><span class="sxs-lookup"><span data-stu-id="2e974-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="2e974-206">Você deve enviar um código de status `202 - Accepted` mesmo que a propriedade clientState não corresponda àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="2e974-206">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="2e974-207">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e974-207">Repeat for other notifications in the request.</span></span>

# <a name="additional-resources"></a><span data-ttu-id="2e974-208">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="2e974-208">Additional resources</span></span>

* [<span data-ttu-id="2e974-209">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-209">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="2e974-210">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-210">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="2e974-211">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="2e974-211">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="2e974-212">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="2e974-212">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="2e974-213">Exemplo de webhooks do Microsoft Graph para ASP,NET</span><span class="sxs-lookup"><span data-stu-id="2e974-213">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

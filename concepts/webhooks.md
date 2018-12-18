---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.
author: piotrci
ms.openlocfilehash: 6af6f3c54a7956d6a505c88bfc82fc8233dccdad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337041"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="ee0b9-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="ee0b9-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="ee0b9-p102">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="ee0b9-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="ee0b9-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="ee0b9-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="ee0b9-112">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="ee0b9-112">Supported resources</span></span>

<span data-ttu-id="ee0b9-113">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="ee0b9-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="ee0b9-114">Messages</span></span>
- <span data-ttu-id="ee0b9-115">Eventos</span><span class="sxs-lookup"><span data-stu-id="ee0b9-115">Events</span></span>
- <span data-ttu-id="ee0b9-116">Contatos</span><span class="sxs-lookup"><span data-stu-id="ee0b9-116">Contacts</span></span>
- <span data-ttu-id="ee0b9-117">Usuários</span><span class="sxs-lookup"><span data-stu-id="ee0b9-117">Users</span></span>
- <span data-ttu-id="ee0b9-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="ee0b9-118">Groups</span></span>
- <span data-ttu-id="ee0b9-119">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="ee0b9-119">Group conversations</span></span>
- <span data-ttu-id="ee0b9-120">Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="ee0b9-120">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="ee0b9-121">Pastas do OneDrive pessoais do usuário</span><span class="sxs-lookup"><span data-stu-id="ee0b9-121">User's personal OneDrive folders</span></span>
- <span data-ttu-id="ee0b9-122">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="ee0b9-122">Security Alerts</span></span>

<span data-ttu-id="ee0b9-123">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="ee0b9-123">For instance, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="ee0b9-124">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="ee0b9-124">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="ee0b9-125">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="ee0b9-125">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="ee0b9-126">Ou para uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="ee0b9-126">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="ee0b9-127">Ou para o OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="ee0b9-127">Or to a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="ee0b9-128">Ou, para um novo [alerta da API de segurança](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="ee0b9-128">Or to a new [Security API alert](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="ee0b9-129">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="ee0b9-129">Azure AD resource limitations</span></span>

<span data-ttu-id="ee0b9-130">Determinados limites se aplicam aos recursos baseados no Microsoft Azure AD (usuários, grupos) e podem gerar erros quando excedidos:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-130">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="ee0b9-131">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-131">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="ee0b9-132">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="ee0b9-132">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="ee0b9-133">Por locatário: total de 35 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="ee0b9-133">Per tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="ee0b9-134">Combinação por aplicativo e locatário: sete assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="ee0b9-134">Per app and tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="ee0b9-135">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-135">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="ee0b9-136">Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-136">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="ee0b9-137">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-137">Subscription lifetime</span></span>

<span data-ttu-id="ee0b9-138">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-138">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="ee0b9-139">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-139">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="ee0b9-140">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-140">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="ee0b9-141">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="ee0b9-141">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="ee0b9-142">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-142">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="ee0b9-143">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="ee0b9-143">Managing subscriptions</span></span>

<span data-ttu-id="ee0b9-144">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-144">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="ee0b9-145">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-145">Creating a subscription</span></span>

<span data-ttu-id="ee0b9-p105">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="ee0b9-148">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-148">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="ee0b9-149">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-149">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="ee0b9-150">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-150">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="ee0b9-151">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-151">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="ee0b9-152">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-152">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="ee0b9-153">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-153">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="ee0b9-154">O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-154">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="ee0b9-155">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-155">Subscription request example</span></span>

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

<span data-ttu-id="ee0b9-156">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-156">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="ee0b9-157">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="ee0b9-157">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="ee0b9-158">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-158">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="ee0b9-159">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-159">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="ee0b9-160">Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-160">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="ee0b9-161">A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-161">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="ee0b9-162">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-162">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="ee0b9-163">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-163">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="ee0b9-164">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="ee0b9-164">Notification endpoint validation</span></span>

<span data-ttu-id="ee0b9-165">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-165">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="ee0b9-166">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-166">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="ee0b9-167">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-167">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="ee0b9-168">**Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-168">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="ee0b9-169">Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-169">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="ee0b9-170">Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-170">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="ee0b9-171">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-171">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="ee0b9-172">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="ee0b9-172">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="ee0b9-173">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-173">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="ee0b9-174">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-174">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="ee0b9-175">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-175">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="ee0b9-176">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-176">Renewing a subscription</span></span>

<span data-ttu-id="ee0b9-177">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-177">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="ee0b9-178">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-178">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="ee0b9-179">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-179">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="ee0b9-180">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-180">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="ee0b9-181">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-181">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="ee0b9-182">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-182">Deleting a subscription</span></span>

<span data-ttu-id="ee0b9-183">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-183">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="ee0b9-184">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-184">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="ee0b9-185">Notificações</span><span class="sxs-lookup"><span data-stu-id="ee0b9-185">Notifications</span></span>

<span data-ttu-id="ee0b9-186">O cliente começa a receber notificações depois de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-186">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="ee0b9-187">O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-187">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="ee0b9-188">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-188">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="ee0b9-189">**Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-189">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="ee0b9-190">Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-190">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="ee0b9-191">Propriedades do objeto notification</span><span class="sxs-lookup"><span data-stu-id="ee0b9-191">Notification properties</span></span>

<span data-ttu-id="ee0b9-192">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-192">The notification object has the following properties:</span></span>

| <span data-ttu-id="ee0b9-193">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee0b9-193">Property</span></span> | <span data-ttu-id="ee0b9-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee0b9-194">Type</span></span> | <span data-ttu-id="ee0b9-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee0b9-195">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ee0b9-196">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="ee0b9-196">subscriptionId</span></span> | <span data-ttu-id="ee0b9-197">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-197">string</span></span> | <span data-ttu-id="ee0b9-198">A ID da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-198">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="ee0b9-199">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee0b9-199">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="ee0b9-200">dateTime</span><span class="sxs-lookup"><span data-stu-id="ee0b9-200">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="ee0b9-201">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-201">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="ee0b9-202">clientState</span><span class="sxs-lookup"><span data-stu-id="ee0b9-202">clientState</span></span> | <span data-ttu-id="ee0b9-203">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-203">string</span></span> | <span data-ttu-id="ee0b9-204">A propriedade `clientState` especificada na solicitação de assinatura. (caso haja).</span><span class="sxs-lookup"><span data-stu-id="ee0b9-204">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="ee0b9-205">changeType</span><span class="sxs-lookup"><span data-stu-id="ee0b9-205">changeType</span></span> | <span data-ttu-id="ee0b9-206">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-206">string</span></span> | <span data-ttu-id="ee0b9-207">O tipo de evento que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-207">The event type that caused the notification.</span></span> <span data-ttu-id="ee0b9-208">Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-208">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="ee0b9-209">recurso</span><span class="sxs-lookup"><span data-stu-id="ee0b9-209">resource</span></span> | <span data-ttu-id="ee0b9-210">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-210">string</span></span> | <span data-ttu-id="ee0b9-211">O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-211">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="ee0b9-212">resourceData</span><span class="sxs-lookup"><span data-stu-id="ee0b9-212">resourceData</span></span> | <span data-ttu-id="ee0b9-213">objeto</span><span class="sxs-lookup"><span data-stu-id="ee0b9-213">object</span></span> | <span data-ttu-id="ee0b9-214">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-214">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="ee0b9-215">Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-215">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="ee0b9-216">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee0b9-216">Property</span></span> | <span data-ttu-id="ee0b9-217">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee0b9-217">Type</span></span> | <span data-ttu-id="ee0b9-218">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee0b9-218">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ee0b9-219">@odata.type</span><span class="sxs-lookup"><span data-stu-id="ee0b9-219">@odata.type</span></span> | <span data-ttu-id="ee0b9-220">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-220">string</span></span> | <span data-ttu-id="ee0b9-221">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-221">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="ee0b9-222">@odata.id</span><span class="sxs-lookup"><span data-stu-id="ee0b9-222">@odata.id</span></span> | <span data-ttu-id="ee0b9-223">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-223">string</span></span> | <span data-ttu-id="ee0b9-224">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-224">The OData identifier of the object.</span></span> |
| <span data-ttu-id="ee0b9-225">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="ee0b9-225">@odata.etag</span></span> | <span data-ttu-id="ee0b9-226">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-226">string</span></span> | <span data-ttu-id="ee0b9-227">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-227">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="ee0b9-228">id</span><span class="sxs-lookup"><span data-stu-id="ee0b9-228">id</span></span> | <span data-ttu-id="ee0b9-229">string</span><span class="sxs-lookup"><span data-stu-id="ee0b9-229">string</span></span> | <span data-ttu-id="ee0b9-230">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-230">The identifier of the object.</span></span> |

> <span data-ttu-id="ee0b9-231">**Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-231">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="ee0b9-232">Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-232">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="ee0b9-233">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="ee0b9-233">Notification example</span></span>

<span data-ttu-id="ee0b9-234">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-234">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="ee0b9-235">Observe que o campo `value` é uma matriz de objetos.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-235">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="ee0b9-236">Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-236">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="ee0b9-237">Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-237">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="ee0b9-238">Processar a notificação</span><span class="sxs-lookup"><span data-stu-id="ee0b9-238">Processing the notification</span></span>

<span data-ttu-id="ee0b9-239">Cada notificação recebida por seu aplicativo deve ser processada.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-239">Each notification received by your app should be processed.</span></span> <span data-ttu-id="ee0b9-240">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="ee0b9-240">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="ee0b9-241">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-241">Validate the `clientState` property.</span></span> <span data-ttu-id="ee0b9-242">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-242">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="ee0b9-243">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-243">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="ee0b9-244">É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-244">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="ee0b9-245">Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-245">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="ee0b9-246">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-246">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="ee0b9-247">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-247">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="ee0b9-248">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-248">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="ee0b9-249">**Observação:** você deve enviar um código de status `202 - Accepted` mesmo que a propriedade `clientState` não corresponda àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-249">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="ee0b9-250">Essa é uma boa prática, uma vez que impede que um possível ator invasor descubra que você não confia nas notificações dele e use as informações para tentar adivinhar o valor da propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-250">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="ee0b9-251">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-251">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="ee0b9-252">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="ee0b9-252">Code samples</span></span>

<span data-ttu-id="ee0b9-253">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="ee0b9-253">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="ee0b9-254">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="ee0b9-254">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="ee0b9-255">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="ee0b9-255">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="ee0b9-256">Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs</span><span class="sxs-lookup"><span data-stu-id="ee0b9-256">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="ee0b9-257">Confira também</span><span class="sxs-lookup"><span data-stu-id="ee0b9-257">See also</span></span>

- [<span data-ttu-id="ee0b9-258">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="ee0b9-259">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="ee0b9-260">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="ee0b9-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0

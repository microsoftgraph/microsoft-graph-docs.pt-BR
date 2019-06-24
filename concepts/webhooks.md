---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 43e4e4893cae46bb5d3bcecc1f0d7e96da4ccfed
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133779"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="fd8fa-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="fd8fa-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="fd8fa-p102">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="fd8fa-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="fd8fa-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="fd8fa-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-111">For example, it fetches more data, updates its cache and views, etc.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="fd8fa-112">Criar um aplicativo webhook com .NET Core</span><span class="sxs-lookup"><span data-stu-id="fd8fa-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

## <a name="supported-resources"></a><span data-ttu-id="fd8fa-113">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="fd8fa-113">Supported resources</span></span>

<span data-ttu-id="fd8fa-114">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-114">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="fd8fa-115">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd8fa-115">Outlook [message][]</span></span>
- <span data-ttu-id="fd8fa-116">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd8fa-116">Outlook [event][]</span></span>
- <span data-ttu-id="fd8fa-117">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd8fa-117">Outlook personal [contact][]</span></span>
- <span data-ttu-id="fd8fa-118">[user][]</span><span class="sxs-lookup"><span data-stu-id="fd8fa-118">[user][]</span></span>
- <span data-ttu-id="fd8fa-119">[group][]</span><span class="sxs-lookup"><span data-stu-id="fd8fa-119">[group][]</span></span>
- <span data-ttu-id="fd8fa-120">[Conversa][] em grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="fd8fa-120">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="fd8fa-121">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="fd8fa-121">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="fd8fa-122">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="fd8fa-122">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="fd8fa-123">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="fd8fa-123">Security [alert][]</span></span>

<span data-ttu-id="fd8fa-124">Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="fd8fa-124">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="fd8fa-125">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="fd8fa-125">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="fd8fa-126">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="fd8fa-126">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="fd8fa-127">Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="fd8fa-127">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="fd8fa-128">Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="fd8fa-128">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="fd8fa-129">Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="fd8fa-129">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="fd8fa-130">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="fd8fa-130">Azure AD resource limitations</span></span>

<span data-ttu-id="fd8fa-131">Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-131">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="fd8fa-132">**Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-132">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="fd8fa-133">Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-133">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="fd8fa-134">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-134">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="fd8fa-135">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="fd8fa-135">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="fd8fa-136">Por locatário: total de 1000 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="fd8fa-136">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="fd8fa-137">Combinação por aplicativo e locatário: 100 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="fd8fa-137">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="fd8fa-138">Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-138">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="fd8fa-139">A propriedade `message` explicará qual limite foi excedido.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-139">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="fd8fa-140">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-140">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="fd8fa-141">Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-141">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="fd8fa-142">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-142">Subscription lifetime</span></span>

<span data-ttu-id="fd8fa-143">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-143">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="fd8fa-144">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-144">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="fd8fa-145">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-145">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="fd8fa-146">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="fd8fa-146">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="fd8fa-147">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-147">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="fd8fa-148">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="fd8fa-148">Managing subscriptions</span></span>

<span data-ttu-id="fd8fa-149">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-149">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="fd8fa-150">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-150">Creating a subscription</span></span>

<span data-ttu-id="fd8fa-p107">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-p107">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="fd8fa-153">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-153">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="fd8fa-154">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-154">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="fd8fa-155">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-155">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="fd8fa-156">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-156">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="fd8fa-157">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-157">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="fd8fa-158">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-158">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="fd8fa-159">O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-159">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="fd8fa-160">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-160">Subscription request example</span></span>

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

<span data-ttu-id="fd8fa-161">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-161">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="fd8fa-162">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fd8fa-162">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="fd8fa-163">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-163">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="fd8fa-164">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-164">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="fd8fa-165">Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-165">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="fd8fa-166">A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-166">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="fd8fa-167">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-167">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="fd8fa-168">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-168">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="fd8fa-169">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="fd8fa-169">Notification endpoint validation</span></span>

<span data-ttu-id="fd8fa-170">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-170">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="fd8fa-171">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-171">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="fd8fa-172">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-172">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="fd8fa-173">**Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-173">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="fd8fa-174">Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-174">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="fd8fa-175">Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-175">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="fd8fa-176">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-176">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="fd8fa-177">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="fd8fa-177">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="fd8fa-178">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-178">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="fd8fa-179">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-179">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="fd8fa-180">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-180">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="fd8fa-181">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-181">Renewing a subscription</span></span>

<span data-ttu-id="fd8fa-182">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-182">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="fd8fa-183">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-183">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="fd8fa-184">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-184">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="fd8fa-185">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-185">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="fd8fa-186">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-186">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="fd8fa-187">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-187">Deleting a subscription</span></span>

<span data-ttu-id="fd8fa-188">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-188">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="fd8fa-189">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-189">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="fd8fa-190">Notificações</span><span class="sxs-lookup"><span data-stu-id="fd8fa-190">Notifications</span></span>

<span data-ttu-id="fd8fa-191">O cliente começa a receber notificações depois de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-191">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="fd8fa-192">O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-192">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="fd8fa-193">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-193">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="fd8fa-194">**Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-194">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="fd8fa-195">Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-195">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="fd8fa-196">Propriedades do objeto notification</span><span class="sxs-lookup"><span data-stu-id="fd8fa-196">Notification properties</span></span>

<span data-ttu-id="fd8fa-197">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-197">The notification object has the following properties:</span></span>

| <span data-ttu-id="fd8fa-198">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd8fa-198">Property</span></span> | <span data-ttu-id="fd8fa-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd8fa-199">Type</span></span> | <span data-ttu-id="fd8fa-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd8fa-200">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fd8fa-201">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="fd8fa-201">subscriptionId</span></span> | <span data-ttu-id="fd8fa-202">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-202">string</span></span> | <span data-ttu-id="fd8fa-203">A ID da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-203">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="fd8fa-204">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd8fa-204">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="fd8fa-205">dateTime</span><span class="sxs-lookup"><span data-stu-id="fd8fa-205">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="fd8fa-206">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-206">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="fd8fa-207">clientState</span><span class="sxs-lookup"><span data-stu-id="fd8fa-207">clientState</span></span> | <span data-ttu-id="fd8fa-208">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-208">string</span></span> | <span data-ttu-id="fd8fa-209">A propriedade `clientState` especificada na solicitação de assinatura. (caso haja).</span><span class="sxs-lookup"><span data-stu-id="fd8fa-209">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="fd8fa-210">changeType</span><span class="sxs-lookup"><span data-stu-id="fd8fa-210">changeType</span></span> | <span data-ttu-id="fd8fa-211">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-211">string</span></span> | <span data-ttu-id="fd8fa-212">O tipo de evento que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-212">The event type that caused the notification.</span></span> <span data-ttu-id="fd8fa-213">Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-213">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="fd8fa-214">recurso</span><span class="sxs-lookup"><span data-stu-id="fd8fa-214">resource</span></span> | <span data-ttu-id="fd8fa-215">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-215">string</span></span> | <span data-ttu-id="fd8fa-216">O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-216">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="fd8fa-217">resourceData</span><span class="sxs-lookup"><span data-stu-id="fd8fa-217">resourceData</span></span> | <span data-ttu-id="fd8fa-218">objeto</span><span class="sxs-lookup"><span data-stu-id="fd8fa-218">object</span></span> | <span data-ttu-id="fd8fa-219">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-219">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="fd8fa-220">Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-220">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="fd8fa-221">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd8fa-221">Property</span></span> | <span data-ttu-id="fd8fa-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd8fa-222">Type</span></span> | <span data-ttu-id="fd8fa-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd8fa-223">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fd8fa-224">@odata.type</span><span class="sxs-lookup"><span data-stu-id="fd8fa-224">@odata.type</span></span> | <span data-ttu-id="fd8fa-225">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-225">string</span></span> | <span data-ttu-id="fd8fa-226">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-226">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="fd8fa-227">@odata.id</span><span class="sxs-lookup"><span data-stu-id="fd8fa-227">@odata.id</span></span> | <span data-ttu-id="fd8fa-228">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-228">string</span></span> | <span data-ttu-id="fd8fa-229">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-229">The OData identifier of the object.</span></span> |
| <span data-ttu-id="fd8fa-230">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="fd8fa-230">@odata.etag</span></span> | <span data-ttu-id="fd8fa-231">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-231">string</span></span> | <span data-ttu-id="fd8fa-232">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-232">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="fd8fa-233">id</span><span class="sxs-lookup"><span data-stu-id="fd8fa-233">id</span></span> | <span data-ttu-id="fd8fa-234">string</span><span class="sxs-lookup"><span data-stu-id="fd8fa-234">string</span></span> | <span data-ttu-id="fd8fa-235">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-235">The identifier of the object.</span></span> |

> <span data-ttu-id="fd8fa-236">**Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-236">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="fd8fa-237">Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-237">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="fd8fa-238">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="fd8fa-238">Notification example</span></span>

<span data-ttu-id="fd8fa-239">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-239">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="fd8fa-240">Observe que o campo `value` é uma matriz de objetos.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-240">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="fd8fa-241">Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-241">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="fd8fa-242">Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-242">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="fd8fa-243">Processar a notificação</span><span class="sxs-lookup"><span data-stu-id="fd8fa-243">Processing the notification</span></span>

<span data-ttu-id="fd8fa-244">Cada notificação recebida por seu aplicativo deve ser processada.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-244">Each notification received by your app should be processed.</span></span> <span data-ttu-id="fd8fa-245">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="fd8fa-245">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="fd8fa-246">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-246">Validate the `clientState` property.</span></span> <span data-ttu-id="fd8fa-247">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-247">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="fd8fa-248">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-248">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="fd8fa-249">É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-249">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="fd8fa-250">Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-250">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="fd8fa-251">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-251">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="fd8fa-252">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-252">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="fd8fa-253">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-253">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="fd8fa-254">**Observação:** você deve enviar um código de status `202 - Accepted` mesmo que a propriedade `clientState` não corresponda àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-254">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="fd8fa-255">Essa é uma boa prática, uma vez que impede que um possível ator invasor descubra que você não confia nas notificações dele e use as informações para tentar adivinhar o valor da propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-255">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="fd8fa-256">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-256">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="fd8fa-257">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="fd8fa-257">Code samples</span></span>

<span data-ttu-id="fd8fa-258">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="fd8fa-258">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="fd8fa-259">Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fd8fa-259">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="fd8fa-260">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="fd8fa-260">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="fd8fa-261">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="fd8fa-261">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="fd8fa-262">Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs</span><span class="sxs-lookup"><span data-stu-id="fd8fa-262">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="fd8fa-263">Confira também</span><span class="sxs-lookup"><span data-stu-id="fd8fa-263">See also</span></span>

- [<span data-ttu-id="fd8fa-264">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-264">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="fd8fa-265">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-265">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="fd8fa-266">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="fd8fa-266">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="fd8fa-267">Alterar tutorial de notificações</span><span class="sxs-lookup"><span data-stu-id="fd8fa-267">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)

[contato]: /graph/api/resources/contact?view=graph-rest-1.0
[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversa]: /graph/api/resources/conversation?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0

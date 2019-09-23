---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.
author: piotrci
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 85d654e6e42a271500ff8d0c2f3181e7d591f3a6
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053890"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="3cf86-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="3cf86-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="3cf86-p102">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="3cf86-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="3cf86-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="3cf86-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="3cf86-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="3cf86-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="3cf86-111">For example, it fetches more data, updates its cache and views, etc.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="3cf86-112">Criar um aplicativo webhook com .NET Core</span><span class="sxs-lookup"><span data-stu-id="3cf86-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

## <a name="supported-resources"></a><span data-ttu-id="3cf86-113">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="3cf86-113">Supported resources</span></span>

<span data-ttu-id="3cf86-114">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="3cf86-114">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="3cf86-115">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="3cf86-115">Outlook [message][]</span></span>
- <span data-ttu-id="3cf86-116">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="3cf86-116">Outlook [event][]</span></span>
- <span data-ttu-id="3cf86-117">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="3cf86-117">Outlook personal [contact][]</span></span>
- <span data-ttu-id="3cf86-118">[user][]</span><span class="sxs-lookup"><span data-stu-id="3cf86-118">[user][]</span></span>
- <span data-ttu-id="3cf86-119">[group][]</span><span class="sxs-lookup"><span data-stu-id="3cf86-119">[group][]</span></span>
- <span data-ttu-id="3cf86-120">[Conversa][] em grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="3cf86-120">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="3cf86-121">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="3cf86-121">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="3cf86-122">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="3cf86-122">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="3cf86-123">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="3cf86-123">Security [alert][]</span></span>

<span data-ttu-id="3cf86-124">Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="3cf86-124">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="3cf86-125">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="3cf86-125">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="3cf86-126">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="3cf86-126">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="3cf86-127">Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="3cf86-127">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="3cf86-128">Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="3cf86-128">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="3cf86-129">Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="3cf86-129">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="3cf86-130">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="3cf86-130">Azure AD resource limitations</span></span>

<span data-ttu-id="3cf86-131">Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:</span><span class="sxs-lookup"><span data-stu-id="3cf86-131">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="3cf86-132">**Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3cf86-132">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="3cf86-133">Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3cf86-133">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="3cf86-134">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="3cf86-134">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="3cf86-135">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="3cf86-135">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="3cf86-136">Por locatário: total de 1000 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="3cf86-136">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="3cf86-137">Combinação por aplicativo e locatário: 100 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="3cf86-137">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="3cf86-138">Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-138">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="3cf86-139">A propriedade `message` explicará qual limite foi excedido.</span><span class="sxs-lookup"><span data-stu-id="3cf86-139">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="3cf86-140">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3cf86-140">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="3cf86-141">Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="3cf86-141">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="3cf86-142">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-142">Subscription lifetime</span></span>

<span data-ttu-id="3cf86-143">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="3cf86-143">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="3cf86-144">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="3cf86-144">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="3cf86-145">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-145">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="3cf86-146">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="3cf86-146">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="3cf86-147">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="3cf86-147">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="3cf86-148">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="3cf86-148">Managing subscriptions</span></span>

<span data-ttu-id="3cf86-149">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="3cf86-149">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="3cf86-150">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-150">Creating a subscription</span></span>

<span data-ttu-id="3cf86-p107">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="3cf86-p107">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="3cf86-153">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="3cf86-153">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="3cf86-154">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-154">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="3cf86-155">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-155">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="3cf86-156">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="3cf86-156">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="3cf86-157">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3cf86-157">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="3cf86-158">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="3cf86-158">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="3cf86-159">O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-159">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="3cf86-160">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-160">Subscription request example</span></span>

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

<span data-ttu-id="3cf86-161">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="3cf86-161">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="3cf86-162">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="3cf86-162">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="3cf86-163">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="3cf86-163">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="3cf86-164">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-164">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="3cf86-165">Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="3cf86-165">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="3cf86-166">A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3cf86-166">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="3cf86-167">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3cf86-167">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="3cf86-168">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="3cf86-168">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="3cf86-169">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="3cf86-169">Notification endpoint validation</span></span>

<span data-ttu-id="3cf86-170">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-170">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="3cf86-171">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="3cf86-171">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="3cf86-172">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="3cf86-172">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="3cf86-173">**Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP.</span><span class="sxs-lookup"><span data-stu-id="3cf86-173">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="3cf86-174">Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="3cf86-174">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="3cf86-175">Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="3cf86-175">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="3cf86-176">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="3cf86-176">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="3cf86-177">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="3cf86-177">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="3cf86-178">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-178">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="3cf86-179">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3cf86-179">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="3cf86-180">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="3cf86-180">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="3cf86-181">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-181">Renewing a subscription</span></span>

<span data-ttu-id="3cf86-182">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-182">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="3cf86-183">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="3cf86-183">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="3cf86-184">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-184">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="3cf86-185">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="3cf86-185">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="3cf86-186">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-186">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="3cf86-187">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-187">Deleting a subscription</span></span>

<span data-ttu-id="3cf86-188">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="3cf86-188">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="3cf86-189">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-189">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="3cf86-190">Notificações</span><span class="sxs-lookup"><span data-stu-id="3cf86-190">Notifications</span></span>

<span data-ttu-id="3cf86-191">O cliente começa a receber notificações depois de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-191">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="3cf86-192">O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="3cf86-192">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="3cf86-193">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-193">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="3cf86-194">**Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes.</span><span class="sxs-lookup"><span data-stu-id="3cf86-194">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="3cf86-195">Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-195">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="3cf86-196">Propriedades do objeto notification</span><span class="sxs-lookup"><span data-stu-id="3cf86-196">Notification properties</span></span>

<span data-ttu-id="3cf86-197">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="3cf86-197">The notification object has the following properties:</span></span>

| <span data-ttu-id="3cf86-198">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cf86-198">Property</span></span> | <span data-ttu-id="3cf86-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cf86-199">Type</span></span> | <span data-ttu-id="3cf86-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf86-200">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="3cf86-201">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="3cf86-201">subscriptionId</span></span> | <span data-ttu-id="3cf86-202">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-202">string</span></span> | <span data-ttu-id="3cf86-203">A ID da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-203">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="3cf86-204">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf86-204">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="3cf86-205">dateTime</span><span class="sxs-lookup"><span data-stu-id="3cf86-205">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="3cf86-206">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-206">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="3cf86-207">clientState</span><span class="sxs-lookup"><span data-stu-id="3cf86-207">clientState</span></span> | <span data-ttu-id="3cf86-208">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-208">string</span></span> | <span data-ttu-id="3cf86-209">A propriedade `clientState` especificada na solicitação de assinatura. (caso haja).</span><span class="sxs-lookup"><span data-stu-id="3cf86-209">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="3cf86-210">changeType</span><span class="sxs-lookup"><span data-stu-id="3cf86-210">changeType</span></span> | <span data-ttu-id="3cf86-211">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-211">string</span></span> | <span data-ttu-id="3cf86-212">O tipo de evento que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-212">The event type that caused the notification.</span></span> <span data-ttu-id="3cf86-213">Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="3cf86-213">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="3cf86-214">recurso</span><span class="sxs-lookup"><span data-stu-id="3cf86-214">resource</span></span> | <span data-ttu-id="3cf86-215">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-215">string</span></span> | <span data-ttu-id="3cf86-216">O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-216">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="3cf86-217">resourceData</span><span class="sxs-lookup"><span data-stu-id="3cf86-217">resourceData</span></span> | <span data-ttu-id="3cf86-218">objeto</span><span class="sxs-lookup"><span data-stu-id="3cf86-218">object</span></span> | <span data-ttu-id="3cf86-219">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="3cf86-219">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="3cf86-220">Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="3cf86-220">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="3cf86-221">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cf86-221">Property</span></span> | <span data-ttu-id="3cf86-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cf86-222">Type</span></span> | <span data-ttu-id="3cf86-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf86-223">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="3cf86-224">@odata.type</span><span class="sxs-lookup"><span data-stu-id="3cf86-224">@odata.type</span></span> | <span data-ttu-id="3cf86-225">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-225">string</span></span> | <span data-ttu-id="3cf86-226">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="3cf86-226">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="3cf86-227">@odata.id</span><span class="sxs-lookup"><span data-stu-id="3cf86-227">@odata.id</span></span> | <span data-ttu-id="3cf86-228">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-228">string</span></span> | <span data-ttu-id="3cf86-229">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="3cf86-229">The OData identifier of the object.</span></span> |
| <span data-ttu-id="3cf86-230">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="3cf86-230">@odata.etag</span></span> | <span data-ttu-id="3cf86-231">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-231">string</span></span> | <span data-ttu-id="3cf86-232">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="3cf86-232">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="3cf86-233">id</span><span class="sxs-lookup"><span data-stu-id="3cf86-233">id</span></span> | <span data-ttu-id="3cf86-234">string</span><span class="sxs-lookup"><span data-stu-id="3cf86-234">string</span></span> | <span data-ttu-id="3cf86-235">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="3cf86-235">The identifier of the object.</span></span> |

> <span data-ttu-id="3cf86-236">**Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada.</span><span class="sxs-lookup"><span data-stu-id="3cf86-236">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="3cf86-237">Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.</span><span class="sxs-lookup"><span data-stu-id="3cf86-237">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="3cf86-238">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="3cf86-238">Notification example</span></span>

<span data-ttu-id="3cf86-239">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="3cf86-239">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="3cf86-240">Observe que o campo `value` é uma matriz de objetos.</span><span class="sxs-lookup"><span data-stu-id="3cf86-240">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="3cf86-241">Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-241">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="3cf86-242">Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-242">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="3cf86-243">Processar a notificação</span><span class="sxs-lookup"><span data-stu-id="3cf86-243">Processing the notification</span></span>

<span data-ttu-id="3cf86-244">Cada notificação recebida por seu aplicativo deve ser processada.</span><span class="sxs-lookup"><span data-stu-id="3cf86-244">Each notification received by your app should be processed.</span></span> <span data-ttu-id="3cf86-245">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="3cf86-245">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="3cf86-246">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3cf86-246">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="3cf86-247">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará publicar a notificação algumas vezes, por um período de aproximadamente 4 horas; depois disso, a notificação será descartada e não será entregue.</span><span class="sxs-lookup"><span data-stu-id="3cf86-247">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the notification a number of times, for a period of about 4 hours; after that, the notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="3cf86-248">**Observação:** Envie um código de status `202 - Accepted` assim que receber a notificação, mesmo antes de validar a sua autenticidade.</span><span class="sxs-lookup"><span data-stu-id="3cf86-248">**Note:** Send a `202 - Accepted` status code as soon as you receive the notification, even before validating its authenticity.</span></span> <span data-ttu-id="3cf86-249">Você está simplesmente confirmando o recebimento da notificação e impedindo tentativas desnecessárias.</span><span class="sxs-lookup"><span data-stu-id="3cf86-249">You are simply acknowledging the receipt of the notification and preventing unnecessary retries.</span></span> <span data-ttu-id="3cf86-250">O tempo limite atual é de 30 segundos, mas pode ser reduzido no futuro para otimizar o desempenho do serviço.</span><span class="sxs-lookup"><span data-stu-id="3cf86-250">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span>

1. <span data-ttu-id="3cf86-251">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="3cf86-251">Validate the `clientState` property.</span></span> <span data-ttu-id="3cf86-252">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="3cf86-252">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="3cf86-253">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="3cf86-253">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="3cf86-254">É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="3cf86-254">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="3cf86-255">Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="3cf86-255">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="3cf86-256">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="3cf86-256">Update your application based on your business logic.</span></span>

<span data-ttu-id="3cf86-257">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf86-257">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="3cf86-258">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="3cf86-258">Code samples</span></span>

<span data-ttu-id="3cf86-259">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="3cf86-259">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="3cf86-260">Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3cf86-260">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="3cf86-261">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="3cf86-261">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="3cf86-262">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="3cf86-262">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="3cf86-263">Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs</span><span class="sxs-lookup"><span data-stu-id="3cf86-263">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="3cf86-264">Confira também</span><span class="sxs-lookup"><span data-stu-id="3cf86-264">See also</span></span>

- [<span data-ttu-id="3cf86-265">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-265">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="3cf86-266">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-266">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="3cf86-267">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="3cf86-267">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="3cf86-268">Alterar tutorial de notificações</span><span class="sxs-lookup"><span data-stu-id="3cf86-268">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)

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

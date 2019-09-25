---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.
author: piotrci
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 26afa7c71708f617038f8d66c64a7f2a65a1c8d9
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113874"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="cb674-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="cb674-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="cb674-p102">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="cb674-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="cb674-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="cb674-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="cb674-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="cb674-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="cb674-111">For example, it fetches more data, updates its cache and views, etc.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="cb674-112">Criar um aplicativo webhook com .NET Core</span><span class="sxs-lookup"><span data-stu-id="cb674-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

## <a name="supported-resources"></a><span data-ttu-id="cb674-113">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="cb674-113">Supported resources</span></span>

<span data-ttu-id="cb674-114">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="cb674-114">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="cb674-115">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="cb674-115">Outlook [message][]</span></span>
- <span data-ttu-id="cb674-116">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="cb674-116">Outlook [event][]</span></span>
- <span data-ttu-id="cb674-117">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="cb674-117">Outlook personal [contact][]</span></span>
- <span data-ttu-id="cb674-118">[user][]</span><span class="sxs-lookup"><span data-stu-id="cb674-118">[user][]</span></span>
- <span data-ttu-id="cb674-119">[group][]</span><span class="sxs-lookup"><span data-stu-id="cb674-119">[group][]</span></span>
- <span data-ttu-id="cb674-120">[Conversa][] em grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="cb674-120">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="cb674-121">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="cb674-121">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="cb674-122">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="cb674-122">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="cb674-123">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="cb674-123">Security [alert][]</span></span>

<span data-ttu-id="cb674-124">Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="cb674-124">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="cb674-125">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="cb674-125">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="cb674-126">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="cb674-126">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="cb674-127">Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="cb674-127">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="cb674-128">Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="cb674-128">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="cb674-129">Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="cb674-129">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="cb674-130">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="cb674-130">Azure AD resource limitations</span></span>

<span data-ttu-id="cb674-131">Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:</span><span class="sxs-lookup"><span data-stu-id="cb674-131">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="cb674-132">**Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cb674-132">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="cb674-133">Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb674-133">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="cb674-134">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="cb674-134">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="cb674-135">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="cb674-135">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="cb674-136">Por locatário: total de 1000 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="cb674-136">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="cb674-137">Combinação por aplicativo e locatário: 100 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="cb674-137">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="cb674-138">Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="cb674-138">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="cb674-139">A propriedade `message` explicará qual limite foi excedido.</span><span class="sxs-lookup"><span data-stu-id="cb674-139">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="cb674-140">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="cb674-140">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="cb674-141">Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="cb674-141">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="cb674-142">Limitações de recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="cb674-142">Outlook resource limitations</span></span>

<span data-ttu-id="cb674-143">Ao se inscrever em recursos do Outlook, tais como **mensagens**, **eventos** ou **contatos**, se você decidir usar o *nome UPN* em um caminho de recurso, a solicitação de assinatura pode falhar caso o UPN contenha um apóstrofo.</span><span class="sxs-lookup"><span data-stu-id="cb674-143">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="cb674-144">Considere usar IDs de usuário de GUID em vez de UPNs para evitar esse problema.</span><span class="sxs-lookup"><span data-stu-id="cb674-144">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="cb674-145">Por exemplo, em vez de usar o caminho de recursos:</span><span class="sxs-lookup"><span data-stu-id="cb674-145">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="cb674-146">Use:</span><span class="sxs-lookup"><span data-stu-id="cb674-146">Use</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="cb674-147">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-147">Subscription lifetime</span></span>

<span data-ttu-id="cb674-148">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="cb674-148">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="cb674-149">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="cb674-149">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="cb674-150">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-150">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="cb674-151">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="cb674-151">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="cb674-152">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="cb674-152">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="cb674-153">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="cb674-153">Managing subscriptions</span></span>

<span data-ttu-id="cb674-154">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="cb674-154">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="cb674-155">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-155">Creating a subscription</span></span>

<span data-ttu-id="cb674-p108">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="cb674-p108">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="cb674-158">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="cb674-158">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="cb674-159">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb674-159">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="cb674-160">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="cb674-160">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="cb674-161">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="cb674-161">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="cb674-162">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb674-162">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="cb674-163">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="cb674-163">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="cb674-164">O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-164">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="cb674-165">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-165">Subscription request example</span></span>

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

<span data-ttu-id="cb674-166">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="cb674-166">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="cb674-167">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="cb674-167">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="cb674-168">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="cb674-168">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="cb674-169">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="cb674-169">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="cb674-170">Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="cb674-170">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="cb674-171">A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb674-171">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="cb674-172">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb674-172">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="cb674-173">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="cb674-173">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="cb674-174">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="cb674-174">Notification endpoint validation</span></span>

<span data-ttu-id="cb674-175">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-175">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="cb674-176">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="cb674-176">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="cb674-177">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="cb674-177">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="cb674-178">**Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP.</span><span class="sxs-lookup"><span data-stu-id="cb674-178">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="cb674-179">Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="cb674-179">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="cb674-180">Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="cb674-180">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="cb674-181">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="cb674-181">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="cb674-182">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="cb674-182">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="cb674-183">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="cb674-183">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="cb674-184">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb674-184">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="cb674-185">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="cb674-185">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="cb674-186">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-186">Renewing a subscription</span></span>

<span data-ttu-id="cb674-187">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb674-187">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="cb674-188">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="cb674-188">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="cb674-189">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-189">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="cb674-190">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="cb674-190">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="cb674-191">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="cb674-191">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="cb674-192">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-192">Deleting a subscription</span></span>

<span data-ttu-id="cb674-193">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="cb674-193">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="cb674-194">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cb674-194">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="cb674-195">Notificações</span><span class="sxs-lookup"><span data-stu-id="cb674-195">Notifications</span></span>

<span data-ttu-id="cb674-196">O cliente começa a receber notificações depois de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-196">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="cb674-197">O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="cb674-197">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="cb674-198">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="cb674-198">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="cb674-199">**Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes.</span><span class="sxs-lookup"><span data-stu-id="cb674-199">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="cb674-200">Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-200">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="cb674-201">Propriedades do objeto notification</span><span class="sxs-lookup"><span data-stu-id="cb674-201">Notification properties</span></span>

<span data-ttu-id="cb674-202">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="cb674-202">The notification object has the following properties:</span></span>

| <span data-ttu-id="cb674-203">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb674-203">Property</span></span> | <span data-ttu-id="cb674-204">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb674-204">Type</span></span> | <span data-ttu-id="cb674-205">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb674-205">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="cb674-206">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="cb674-206">subscriptionId</span></span> | <span data-ttu-id="cb674-207">string</span><span class="sxs-lookup"><span data-stu-id="cb674-207">string</span></span> | <span data-ttu-id="cb674-208">A ID da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="cb674-208">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="cb674-209">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cb674-209">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="cb674-210">dateTime</span><span class="sxs-lookup"><span data-stu-id="cb674-210">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="cb674-211">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-211">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="cb674-212">clientState</span><span class="sxs-lookup"><span data-stu-id="cb674-212">clientState</span></span> | <span data-ttu-id="cb674-213">string</span><span class="sxs-lookup"><span data-stu-id="cb674-213">string</span></span> | <span data-ttu-id="cb674-214">A propriedade `clientState` especificada na solicitação de assinatura. (caso haja).</span><span class="sxs-lookup"><span data-stu-id="cb674-214">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="cb674-215">changeType</span><span class="sxs-lookup"><span data-stu-id="cb674-215">changeType</span></span> | <span data-ttu-id="cb674-216">string</span><span class="sxs-lookup"><span data-stu-id="cb674-216">string</span></span> | <span data-ttu-id="cb674-217">O tipo de evento que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="cb674-217">The event type that caused the notification.</span></span> <span data-ttu-id="cb674-218">Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="cb674-218">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="cb674-219">recurso</span><span class="sxs-lookup"><span data-stu-id="cb674-219">resource</span></span> | <span data-ttu-id="cb674-220">string</span><span class="sxs-lookup"><span data-stu-id="cb674-220">string</span></span> | <span data-ttu-id="cb674-221">O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="cb674-221">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="cb674-222">resourceData</span><span class="sxs-lookup"><span data-stu-id="cb674-222">resourceData</span></span> | <span data-ttu-id="cb674-223">objeto</span><span class="sxs-lookup"><span data-stu-id="cb674-223">object</span></span> | <span data-ttu-id="cb674-224">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="cb674-224">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="cb674-225">Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="cb674-225">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="cb674-226">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb674-226">Property</span></span> | <span data-ttu-id="cb674-227">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb674-227">Type</span></span> | <span data-ttu-id="cb674-228">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb674-228">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="cb674-229">@odata.type</span><span class="sxs-lookup"><span data-stu-id="cb674-229">@odata.type</span></span> | <span data-ttu-id="cb674-230">string</span><span class="sxs-lookup"><span data-stu-id="cb674-230">string</span></span> | <span data-ttu-id="cb674-231">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="cb674-231">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="cb674-232">@odata.id</span><span class="sxs-lookup"><span data-stu-id="cb674-232">@odata.id</span></span> | <span data-ttu-id="cb674-233">string</span><span class="sxs-lookup"><span data-stu-id="cb674-233">string</span></span> | <span data-ttu-id="cb674-234">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="cb674-234">The OData identifier of the object.</span></span> |
| <span data-ttu-id="cb674-235">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="cb674-235">@odata.etag</span></span> | <span data-ttu-id="cb674-236">string</span><span class="sxs-lookup"><span data-stu-id="cb674-236">string</span></span> | <span data-ttu-id="cb674-237">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="cb674-237">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="cb674-238">id</span><span class="sxs-lookup"><span data-stu-id="cb674-238">id</span></span> | <span data-ttu-id="cb674-239">string</span><span class="sxs-lookup"><span data-stu-id="cb674-239">string</span></span> | <span data-ttu-id="cb674-240">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="cb674-240">The identifier of the object.</span></span> |

> <span data-ttu-id="cb674-241">**Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada.</span><span class="sxs-lookup"><span data-stu-id="cb674-241">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="cb674-242">Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.</span><span class="sxs-lookup"><span data-stu-id="cb674-242">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="cb674-243">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="cb674-243">Notification example</span></span>

<span data-ttu-id="cb674-244">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="cb674-244">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="cb674-245">Observe que o campo `value` é uma matriz de objetos.</span><span class="sxs-lookup"><span data-stu-id="cb674-245">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="cb674-246">Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb674-246">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="cb674-247">Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.</span><span class="sxs-lookup"><span data-stu-id="cb674-247">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="cb674-248">Processar a notificação</span><span class="sxs-lookup"><span data-stu-id="cb674-248">Processing the notification</span></span>

<span data-ttu-id="cb674-249">Cada notificação recebida por seu aplicativo deve ser processada.</span><span class="sxs-lookup"><span data-stu-id="cb674-249">Each notification received by your app should be processed.</span></span> <span data-ttu-id="cb674-250">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="cb674-250">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="cb674-251">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb674-251">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="cb674-252">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará publicar a notificação algumas vezes, por um período de aproximadamente 4 horas; depois disso, a notificação será descartada e não será entregue.</span><span class="sxs-lookup"><span data-stu-id="cb674-252">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the notification a number of times, for a period of about 4 hours; after that, the notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="cb674-253">**Observação:** Envie um código de status `202 - Accepted` assim que receber a notificação, mesmo antes de validar a sua autenticidade.</span><span class="sxs-lookup"><span data-stu-id="cb674-253">**Note:** Send a `202 - Accepted` status code as soon as you receive the notification, even before validating its authenticity.</span></span> <span data-ttu-id="cb674-254">Você está simplesmente confirmando o recebimento da notificação e impedindo tentativas desnecessárias.</span><span class="sxs-lookup"><span data-stu-id="cb674-254">You are simply acknowledging the receipt of the notification and preventing unnecessary retries.</span></span> <span data-ttu-id="cb674-255">O tempo limite atual é de 30 segundos, mas pode ser reduzido no futuro para otimizar o desempenho do serviço.</span><span class="sxs-lookup"><span data-stu-id="cb674-255">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span>

1. <span data-ttu-id="cb674-256">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="cb674-256">Validate the `clientState` property.</span></span> <span data-ttu-id="cb674-257">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="cb674-257">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="cb674-258">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="cb674-258">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="cb674-259">É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="cb674-259">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="cb674-260">Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="cb674-260">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="cb674-261">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="cb674-261">Update your application based on your business logic.</span></span>

<span data-ttu-id="cb674-262">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb674-262">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="cb674-263">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="cb674-263">Code samples</span></span>

<span data-ttu-id="cb674-264">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="cb674-264">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="cb674-265">Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cb674-265">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="cb674-266">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="cb674-266">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="cb674-267">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="cb674-267">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="cb674-268">Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs</span><span class="sxs-lookup"><span data-stu-id="cb674-268">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="cb674-269">Confira também</span><span class="sxs-lookup"><span data-stu-id="cb674-269">See also</span></span>

- [<span data-ttu-id="cb674-270">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-270">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="cb674-271">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-271">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="cb674-272">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="cb674-272">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="cb674-273">Alterar tutorial de notificações</span><span class="sxs-lookup"><span data-stu-id="cb674-273">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)

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

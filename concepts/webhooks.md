---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 54775b566c26f0b6bc99fd1a8482fe5b12c5d1fa
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41651761"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="fd457-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="fd457-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="fd457-p102">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="fd457-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="fd457-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="fd457-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="fd457-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="fd457-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="fd457-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="fd457-112">Criar um aplicativo webhook com .NET Core</span><span class="sxs-lookup"><span data-stu-id="fd457-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

<span data-ttu-id="fd457-113">Por padrão, as notificações de alteração não contêm dados de recursos, exceto o `id`.</span><span class="sxs-lookup"><span data-stu-id="fd457-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="fd457-114">Se o aplicativo exigir dados de recursos, ele poderá fazer chamadas para as APIs do Microsoft Graph para obter o recurso completo.</span><span class="sxs-lookup"><span data-stu-id="fd457-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="fd457-115">Este artigo usa o recurso de **usuário** como um exemplo para trabalhar com notificações.</span><span class="sxs-lookup"><span data-stu-id="fd457-115">This article uses the **user** resource as an example for working with notifications.</span></span>

<span data-ttu-id="fd457-116">Um aplicativo também pode se inscrever para alterar notificações que incluem dados de recursos, para evitar a necessidade de fazer chamadas de API adicionais para acessar os dados.</span><span class="sxs-lookup"><span data-stu-id="fd457-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="fd457-117">Esses aplicativos precisarão implementar um código extra para lidar com os requisitos de tais notificações, especificamente: responder às notificações do ciclo de vida da assinatura, validar a autenticidade das notificações e descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd457-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="fd457-118">Mais tipos de recursos terão suporte para esse tipo de notificações no futuro.</span><span class="sxs-lookup"><span data-stu-id="fd457-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="fd457-119">Para saber mais sobre como trabalhar com essas notificações, confira [Configurar notificações de alteração que incluem dados de recurso (visualização)](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="fd457-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="fd457-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="fd457-120">Supported resources</span></span>

<span data-ttu-id="fd457-121">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="fd457-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="fd457-122">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd457-122">Outlook [message][]</span></span>
- <span data-ttu-id="fd457-123">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd457-123">Outlook [event][]</span></span>
- <span data-ttu-id="fd457-124">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd457-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="fd457-125">[user][]</span><span class="sxs-lookup"><span data-stu-id="fd457-125">[user][]</span></span>
- <span data-ttu-id="fd457-126">[group][]</span><span class="sxs-lookup"><span data-stu-id="fd457-126">[group][]</span></span>
- <span data-ttu-id="fd457-127">[Conversa][] em grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="fd457-127">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="fd457-128">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="fd457-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="fd457-129">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="fd457-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="fd457-130">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="fd457-130">Security [alert][]</span></span>

<span data-ttu-id="fd457-131">Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="fd457-131">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="fd457-132">Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`</span><span class="sxs-lookup"><span data-stu-id="fd457-132">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="fd457-133">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="fd457-133">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="fd457-134">Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="fd457-134">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="fd457-135">Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="fd457-135">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="fd457-136">Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="fd457-136">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="fd457-137">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="fd457-137">Azure AD resource limitations</span></span>

<span data-ttu-id="fd457-138">Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:</span><span class="sxs-lookup"><span data-stu-id="fd457-138">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="fd457-139">**Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd457-139">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="fd457-140">Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd457-140">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="fd457-141">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="fd457-141">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="fd457-142">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="fd457-142">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="fd457-143">Por locatário: total de 1000 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="fd457-143">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="fd457-144">Combinação por aplicativo e locatário: 100 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="fd457-144">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="fd457-145">Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="fd457-145">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="fd457-146">A propriedade `message` explicará qual limite foi excedido.</span><span class="sxs-lookup"><span data-stu-id="fd457-146">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="fd457-147">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fd457-147">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="fd457-148">Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="fd457-148">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="fd457-149">Limitações de recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="fd457-149">Outlook resource limitations</span></span>

<span data-ttu-id="fd457-150">Ao se inscrever em recursos do Outlook, tais como **mensagens**, **eventos** ou **contatos**, se você decidir usar o *nome UPN* em um caminho de recurso, a solicitação de assinatura pode falhar caso o UPN contenha um apóstrofo.</span><span class="sxs-lookup"><span data-stu-id="fd457-150">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="fd457-151">Considere usar IDs de usuário de GUID em vez de UPNs para evitar esse problema.</span><span class="sxs-lookup"><span data-stu-id="fd457-151">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="fd457-152">Por exemplo, em vez de usar o caminho de recursos:</span><span class="sxs-lookup"><span data-stu-id="fd457-152">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="fd457-153">Use:</span><span class="sxs-lookup"><span data-stu-id="fd457-153">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="fd457-154">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-154">Subscription lifetime</span></span>

<span data-ttu-id="fd457-155">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="fd457-155">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="fd457-156">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="fd457-156">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="fd457-157">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-157">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="fd457-158">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="fd457-158">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="fd457-159">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.</span><span class="sxs-lookup"><span data-stu-id="fd457-159">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="fd457-160">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="fd457-160">Managing subscriptions</span></span>

<span data-ttu-id="fd457-161">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="fd457-161">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="fd457-162">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-162">Creating a subscription</span></span>

<span data-ttu-id="fd457-p110">Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="fd457-p110">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="fd457-165">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="fd457-165">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="fd457-166">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd457-166">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="fd457-167">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="fd457-167">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="fd457-168">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="fd457-168">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="fd457-169">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd457-169">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="fd457-170">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="fd457-170">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="fd457-171">O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-171">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="fd457-172">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-172">Subscription request example</span></span>

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

<span data-ttu-id="fd457-173">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="fd457-173">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="fd457-174">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fd457-174">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="fd457-175">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="fd457-175">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="fd457-176">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="fd457-176">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="fd457-177">Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.</span><span class="sxs-lookup"><span data-stu-id="fd457-177">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="fd457-178">A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd457-178">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="fd457-179">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd457-179">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="fd457-180">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="fd457-180">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="fd457-181">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="fd457-181">Notification endpoint validation</span></span>

<span data-ttu-id="fd457-182">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-182">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="fd457-183">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="fd457-183">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="fd457-184">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="fd457-184">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="fd457-185">**Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP.</span><span class="sxs-lookup"><span data-stu-id="fd457-185">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="fd457-186">Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="fd457-186">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="fd457-187">Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="fd457-187">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="fd457-188">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="fd457-188">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="fd457-189">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="fd457-189">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="fd457-190">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="fd457-190">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="fd457-191">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd457-191">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="fd457-192">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="fd457-192">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="fd457-193">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-193">Renewing a subscription</span></span>

<span data-ttu-id="fd457-194">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd457-194">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="fd457-195">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="fd457-195">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="fd457-196">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-196">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="fd457-197">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="fd457-197">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="fd457-198">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="fd457-198">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="fd457-199">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-199">Deleting a subscription</span></span>

<span data-ttu-id="fd457-200">O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="fd457-200">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="fd457-201">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fd457-201">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="fd457-202">Notificações</span><span class="sxs-lookup"><span data-stu-id="fd457-202">Notifications</span></span>

<span data-ttu-id="fd457-203">O cliente começa a receber notificações depois de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-203">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="fd457-204">O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="fd457-204">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="fd457-205">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="fd457-205">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="fd457-206">**Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes.</span><span class="sxs-lookup"><span data-stu-id="fd457-206">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="fd457-207">Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-207">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="fd457-208">Propriedades do objeto notification</span><span class="sxs-lookup"><span data-stu-id="fd457-208">Notification properties</span></span>

<span data-ttu-id="fd457-209">O objeto notification tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="fd457-209">The notification object has the following properties:</span></span>

| <span data-ttu-id="fd457-210">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd457-210">Property</span></span> | <span data-ttu-id="fd457-211">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd457-211">Type</span></span> | <span data-ttu-id="fd457-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd457-212">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fd457-213">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="fd457-213">subscriptionId</span></span> | <span data-ttu-id="fd457-214">string</span><span class="sxs-lookup"><span data-stu-id="fd457-214">string</span></span> | <span data-ttu-id="fd457-215">A ID da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="fd457-215">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="fd457-216">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd457-216">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="fd457-217">dateTime</span><span class="sxs-lookup"><span data-stu-id="fd457-217">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="fd457-218">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-218">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="fd457-219">clientState</span><span class="sxs-lookup"><span data-stu-id="fd457-219">clientState</span></span> | <span data-ttu-id="fd457-220">string</span><span class="sxs-lookup"><span data-stu-id="fd457-220">string</span></span> | <span data-ttu-id="fd457-221">A propriedade `clientState` especificada na solicitação de assinatura. (caso haja).</span><span class="sxs-lookup"><span data-stu-id="fd457-221">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="fd457-222">changeType</span><span class="sxs-lookup"><span data-stu-id="fd457-222">changeType</span></span> | <span data-ttu-id="fd457-223">string</span><span class="sxs-lookup"><span data-stu-id="fd457-223">string</span></span> | <span data-ttu-id="fd457-224">O tipo de evento que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="fd457-224">The event type that caused the notification.</span></span> <span data-ttu-id="fd457-225">Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida.</span><span class="sxs-lookup"><span data-stu-id="fd457-225">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="fd457-226">recurso</span><span class="sxs-lookup"><span data-stu-id="fd457-226">resource</span></span> | <span data-ttu-id="fd457-227">string</span><span class="sxs-lookup"><span data-stu-id="fd457-227">string</span></span> | <span data-ttu-id="fd457-228">O URI do recurso relativo a `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="fd457-228">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="fd457-229">resourceData</span><span class="sxs-lookup"><span data-stu-id="fd457-229">resourceData</span></span> | <span data-ttu-id="fd457-230">objeto</span><span class="sxs-lookup"><span data-stu-id="fd457-230">object</span></span> | <span data-ttu-id="fd457-231">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="fd457-231">The content of this property depends on the type of resource being subscribed to.</span></span> |
| <span data-ttu-id="fd457-232">tenantId</span><span class="sxs-lookup"><span data-stu-id="fd457-232">tenantId</span></span> | <span data-ttu-id="fd457-233">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd457-233">string</span></span> | <span data-ttu-id="fd457-234">A ID do locatário do qual a notificação se originou.</span><span class="sxs-lookup"><span data-stu-id="fd457-234">The ID of the tenant the notification originated from.</span></span> |

<span data-ttu-id="fd457-235">Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="fd457-235">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="fd457-236">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd457-236">Property</span></span> | <span data-ttu-id="fd457-237">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd457-237">Type</span></span> | <span data-ttu-id="fd457-238">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd457-238">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fd457-239">@odata.type</span><span class="sxs-lookup"><span data-stu-id="fd457-239">@odata.type</span></span> | <span data-ttu-id="fd457-240">string</span><span class="sxs-lookup"><span data-stu-id="fd457-240">string</span></span> | <span data-ttu-id="fd457-241">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="fd457-241">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="fd457-242">@odata.id</span><span class="sxs-lookup"><span data-stu-id="fd457-242">@odata.id</span></span> | <span data-ttu-id="fd457-243">string</span><span class="sxs-lookup"><span data-stu-id="fd457-243">string</span></span> | <span data-ttu-id="fd457-244">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd457-244">The OData identifier of the object.</span></span> |
| <span data-ttu-id="fd457-245">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="fd457-245">@odata.etag</span></span> | <span data-ttu-id="fd457-246">string</span><span class="sxs-lookup"><span data-stu-id="fd457-246">string</span></span> | <span data-ttu-id="fd457-247">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd457-247">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="fd457-248">id</span><span class="sxs-lookup"><span data-stu-id="fd457-248">id</span></span> | <span data-ttu-id="fd457-249">string</span><span class="sxs-lookup"><span data-stu-id="fd457-249">string</span></span> | <span data-ttu-id="fd457-250">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd457-250">The identifier of the object.</span></span> |

> <span data-ttu-id="fd457-251">**Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada.</span><span class="sxs-lookup"><span data-stu-id="fd457-251">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="fd457-252">Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.</span><span class="sxs-lookup"><span data-stu-id="fd457-252">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="fd457-253">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="fd457-253">Notification example</span></span>

<span data-ttu-id="fd457-254">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="fd457-254">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
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

<span data-ttu-id="fd457-255">Observe que o campo `value` é uma matriz de objetos.</span><span class="sxs-lookup"><span data-stu-id="fd457-255">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="fd457-256">Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd457-256">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="fd457-257">Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.</span><span class="sxs-lookup"><span data-stu-id="fd457-257">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="fd457-258">Processar a notificação</span><span class="sxs-lookup"><span data-stu-id="fd457-258">Processing the notification</span></span>

<span data-ttu-id="fd457-259">Cada notificação recebida por seu aplicativo deve ser processada.</span><span class="sxs-lookup"><span data-stu-id="fd457-259">Each notification received by your app should be processed.</span></span> <span data-ttu-id="fd457-260">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:</span><span class="sxs-lookup"><span data-stu-id="fd457-260">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="fd457-261">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd457-261">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="fd457-262">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará publicar a notificação algumas vezes, por um período de aproximadamente 4 horas; depois disso, a notificação será descartada e não será entregue.</span><span class="sxs-lookup"><span data-stu-id="fd457-262">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the notification a number of times, for a period of about 4 hours; after that, the notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="fd457-263">**Observação:** Envie um código de status `202 - Accepted` assim que receber a notificação, mesmo antes de validar a sua autenticidade.</span><span class="sxs-lookup"><span data-stu-id="fd457-263">**Note:** Send a `202 - Accepted` status code as soon as you receive the notification, even before validating its authenticity.</span></span> <span data-ttu-id="fd457-264">Você está simplesmente confirmando o recebimento da notificação e impedindo tentativas desnecessárias.</span><span class="sxs-lookup"><span data-stu-id="fd457-264">You are simply acknowledging the receipt of the notification and preventing unnecessary retries.</span></span> <span data-ttu-id="fd457-265">O tempo limite atual é de 30 segundos, mas pode ser reduzido no futuro para otimizar o desempenho do serviço.</span><span class="sxs-lookup"><span data-stu-id="fd457-265">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span>

1. <span data-ttu-id="fd457-266">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="fd457-266">Validate the `clientState` property.</span></span> <span data-ttu-id="fd457-267">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd457-267">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="fd457-268">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="fd457-268">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="fd457-269">É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="fd457-269">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="fd457-270">Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="fd457-270">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="fd457-271">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="fd457-271">Update your application based on your business logic.</span></span>

<span data-ttu-id="fd457-272">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd457-272">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="fd457-273">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="fd457-273">Code samples</span></span>

<span data-ttu-id="fd457-274">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="fd457-274">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="fd457-275">Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fd457-275">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="fd457-276">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="fd457-276">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="fd457-277">Exemplo de webhooks do Microsoft Graph para ASP.NET</span><span class="sxs-lookup"><span data-stu-id="fd457-277">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="fd457-278">Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs</span><span class="sxs-lookup"><span data-stu-id="fd457-278">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="fd457-279">Confira também</span><span class="sxs-lookup"><span data-stu-id="fd457-279">See also</span></span>

- [<span data-ttu-id="fd457-280">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-280">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="fd457-281">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-281">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="fd457-282">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="fd457-282">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="fd457-283">Alterar tutorial de notificações</span><span class="sxs-lookup"><span data-stu-id="fd457-283">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)
- [<span data-ttu-id="fd457-284">Notificações do ciclo de vida (visualização)</span><span class="sxs-lookup"><span data-stu-id="fd457-284">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

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

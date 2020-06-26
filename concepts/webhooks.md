---
title: Configurar notificações para alterações nos dados de usuário
description: The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 295f62aeba919fde1384642755b0c51816527d91
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897075"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="7787d-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="7787d-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="7787d-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span><span class="sxs-lookup"><span data-stu-id="7787d-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="7787d-107">A client is a web service that configures its own URL to receive change notifications.</span><span class="sxs-lookup"><span data-stu-id="7787d-107">A client is a web service that configures its own URL to receive change notifications.</span></span> <span data-ttu-id="7787d-108">Client apps use change notifications to update their state upon changes.</span><span class="sxs-lookup"><span data-stu-id="7787d-108">Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="7787d-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações de alteração para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="7787d-109">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="7787d-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="7787d-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="7787d-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="7787d-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="7787d-112">Tutorial: usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7787d-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="7787d-113">Por padrão, as notificações de alteração não contêm dados de recursos, exceto o `id`.</span><span class="sxs-lookup"><span data-stu-id="7787d-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="7787d-114">Se o aplicativo exigir dados de recursos, ele poderá fazer chamadas para as APIs do Microsoft Graph para obter o recurso completo.</span><span class="sxs-lookup"><span data-stu-id="7787d-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="7787d-115">Este artigo usa o recurso **User** como um exemplo para trabalhar com notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="7787d-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="7787d-116">Um aplicativo também pode se inscrever para alterar notificações que incluem dados de recursos, para evitar a necessidade de fazer chamadas de API adicionais para acessar os dados.</span><span class="sxs-lookup"><span data-stu-id="7787d-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="7787d-117">Esses aplicativos precisarão implementar um código extra para lidar com os requisitos de tais notificações, especificamente: responder às notificações do ciclo de vida da assinatura, validar a autenticidade das notificações e descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="7787d-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="7787d-118">Mais tipos de recursos terão suporte para esse tipo de notificações no futuro.</span><span class="sxs-lookup"><span data-stu-id="7787d-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="7787d-119">Para saber mais sobre como trabalhar com essas notificações, confira [Configurar notificações de alteração que incluem dados de recurso (visualização)](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="7787d-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="7787d-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="7787d-120">Supported resources</span></span>

<span data-ttu-id="7787d-121">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="7787d-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="7787d-122">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="7787d-122">Outlook [message][]</span></span>
- <span data-ttu-id="7787d-123">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="7787d-123">Outlook [event][]</span></span>
- <span data-ttu-id="7787d-124">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="7787d-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="7787d-125">[user][]</span><span class="sxs-lookup"><span data-stu-id="7787d-125">[user][]</span></span>
- <span data-ttu-id="7787d-126">[group][]</span><span class="sxs-lookup"><span data-stu-id="7787d-126">[group][]</span></span>
- <span data-ttu-id="7787d-127">[Conversa][] de grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7787d-127">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="7787d-128">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="7787d-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="7787d-129">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="7787d-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="7787d-130">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="7787d-130">Security [alert][]</span></span>
- <span data-ttu-id="7787d-131">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="7787d-131">Teams [callRecord][]</span></span>
- <span data-ttu-id="7787d-132">[chatMessage][] do Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="7787d-132">Teams [chatMessage][] (preview)</span></span>

<span data-ttu-id="7787d-133">Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="7787d-133">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="7787d-134">Ou para um recurso de nível superior:,,,, `/me/messages` `/me/contacts` `/me/events` `users` `groups` ou`/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="7787d-134">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, or `/communications/callRecords`</span></span>

<span data-ttu-id="7787d-135">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="7787d-135">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="7787d-136">Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="7787d-136">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="7787d-137">Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="7787d-137">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="7787d-138">Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="7787d-138">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="7787d-139">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="7787d-139">Azure AD resource limitations</span></span>

<span data-ttu-id="7787d-140">Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:</span><span class="sxs-lookup"><span data-stu-id="7787d-140">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="7787d-141">**Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7787d-141">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="7787d-142">Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-142">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="7787d-143">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="7787d-143">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="7787d-144">Por aplicativo: total de 50 mil assinaturas</span><span class="sxs-lookup"><span data-stu-id="7787d-144">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="7787d-145">Por locatário: total de 1000 assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="7787d-145">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="7787d-146">Combinação por aplicativo e locatário: 100 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="7787d-146">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="7787d-147">Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="7787d-147">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="7787d-148">A propriedade `message` explicará qual limite foi excedido.</span><span class="sxs-lookup"><span data-stu-id="7787d-148">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="7787d-149">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="7787d-149">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="7787d-150">A notificação Changfe para entidades de usuário não tem suporte para contas pessoais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7787d-150">Changfe notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="7787d-151">Existe um [problema conhecido](known-issues.md#change-notifications) nas assinaturas de usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="7787d-151">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="7787d-152">Limitações de recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="7787d-152">Outlook resource limitations</span></span>

<span data-ttu-id="7787d-153">Ao se inscrever em recursos do Outlook, tais como **mensagens**, **eventos** ou **contatos**, se você decidir usar o *nome UPN* em um caminho de recurso, a solicitação de assinatura pode falhar caso o UPN contenha um apóstrofo.</span><span class="sxs-lookup"><span data-stu-id="7787d-153">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="7787d-154">Considere usar IDs de usuário de GUID em vez de UPNs para evitar esse problema.</span><span class="sxs-lookup"><span data-stu-id="7787d-154">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="7787d-155">Por exemplo, em vez de usar o caminho de recursos:</span><span class="sxs-lookup"><span data-stu-id="7787d-155">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="7787d-156">Use:</span><span class="sxs-lookup"><span data-stu-id="7787d-156">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="7787d-157">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-157">Subscription lifetime</span></span>

<span data-ttu-id="7787d-158">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="7787d-158">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="7787d-159">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="7787d-159">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="7787d-160">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="7787d-160">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="7787d-161">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="7787d-161">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="7787d-162">Os aplicativos também podem cancelar a assinatura a qualquer momento para parar de receber notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="7787d-162">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="7787d-163">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="7787d-163">Managing subscriptions</span></span>

<span data-ttu-id="7787d-164">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="7787d-164">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="7787d-165">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-165">Creating a subscription</span></span>

<span data-ttu-id="7787d-166">Creating a subscription is the first step to start receiving change notifications for a resource.</span><span class="sxs-lookup"><span data-stu-id="7787d-166">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="7787d-167">The subscription process is as follows:</span><span class="sxs-lookup"><span data-stu-id="7787d-167">The subscription process is as follows:</span></span>

1. <span data-ttu-id="7787d-168">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="7787d-168">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="7787d-169">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7787d-169">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="7787d-170">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="7787d-170">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="7787d-171">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="7787d-171">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="7787d-172">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-172">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="7787d-173">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="7787d-173">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="7787d-174">O cliente deve armazenar a ID da assinatura para correlacionar notificações de alteração à assinatura.</span><span class="sxs-lookup"><span data-stu-id="7787d-174">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="7787d-175">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-175">Subscription request example</span></span>

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

<span data-ttu-id="7787d-176">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="7787d-176">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="7787d-177">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="7787d-177">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="7787d-178">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="7787d-178">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="7787d-179">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="7787d-179">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="7787d-180">Embora `clientState` não seja necessário, você deve incluí-lo para estar em conformidade com o processo de tratamento de notificação de alterações recomendado.</span><span class="sxs-lookup"><span data-stu-id="7787d-180">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="7787d-181">A definição dessa propriedade permitirá que você confirme se as notificações de alteração recebidas são originadas do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-181">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="7787d-182">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-182">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="7787d-183">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="7787d-183">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="7787d-184">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="7787d-184">Notification endpoint validation</span></span>

<span data-ttu-id="7787d-185">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="7787d-185">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="7787d-186">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="7787d-186">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="7787d-187">O Microsoft Graph envia uma solicitação POST para a URL de notificação:</span><span class="sxs-lookup"><span data-stu-id="7787d-187">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="7787d-188">**Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP.</span><span class="sxs-lookup"><span data-stu-id="7787d-188">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="7787d-189">Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="7787d-189">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="7787d-190">Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="7787d-190">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="7787d-191">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:</span><span class="sxs-lookup"><span data-stu-id="7787d-191">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="7787d-192">Um código de status 200 (OK).</span><span class="sxs-lookup"><span data-stu-id="7787d-192">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="7787d-193">O tipo de conteúdo deve ser `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="7787d-193">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="7787d-194">O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-194">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="7787d-195">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="7787d-195">The client should discard the validation token after providing it in the response.</span></span>

<span data-ttu-id="7787d-196">Além disso, você pode usar a [coleção do Microsoft Graph Postman](use-postman.md) para confirmar que o ponto de extremidade implementa a solicitação de validação.</span><span class="sxs-lookup"><span data-stu-id="7787d-196">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="7787d-197">A solicitação de **Validação de Assinaturas** na pasta **Diversos** fornece testes de unidade que validam a resposta fornecida por seu ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7787d-197">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![resultados do teste de resposta de validação](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="7787d-199">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-199">Renewing a subscription</span></span>

<span data-ttu-id="7787d-200">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7787d-200">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="7787d-201">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="7787d-201">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="7787d-202">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-202">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="7787d-203">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="7787d-203">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="7787d-204">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="7787d-204">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="7787d-205">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-205">Deleting a subscription</span></span>

<span data-ttu-id="7787d-206">O cliente pode parar de receber notificações de alteração excluindo a assinatura usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="7787d-206">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="7787d-207">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7787d-207">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="7787d-208">Notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="7787d-208">Change notifications</span></span>

<span data-ttu-id="7787d-209">Com uma assinatura de cliente para alterações em um recurso, o Microsoft Graph envia uma `POST` solicitação para a URL de notificação sempre que o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="7787d-209">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="7787d-210">Ele envia notificações somente para alterações do tipo especificado na assinatura, por exemplo, `created` .</span><span class="sxs-lookup"><span data-stu-id="7787d-210">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="7787d-211">**Observação:** Se um cliente tiver várias assinaturas que monitoram o mesmo recurso e usarem a mesma URL de notificação, o Microsoft Graph poderá enviar várias notificações de alteração que correspondam a diferentes assinaturas, cada uma mostrando a ID de assinatura correspondente.</span><span class="sxs-lookup"><span data-stu-id="7787d-211">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="7787d-212">Não há garantia de que todas as notificações de alteração na `POST` solicitação pertencem a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="7787d-212">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="7787d-213">Exemplo de notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="7787d-213">Change notification example</span></span>

<span data-ttu-id="7787d-214">Esta seção mostra um exemplo de uma notificação para a criação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="7787d-214">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="7787d-215">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação de alteração, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7787d-215">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="7787d-216">Observe que a notificação está em uma coleção representada no `value` campo.</span><span class="sxs-lookup"><span data-stu-id="7787d-216">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="7787d-217">Consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection) para obter detalhes da carga de notificação.</span><span class="sxs-lookup"><span data-stu-id="7787d-217">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="7787d-218">Quando muitas alterações ocorrem, o Microsoft Graph pode enviar várias notificações que correspondem a diferentes assinaturas na mesma `POST` solicitação.</span><span class="sxs-lookup"><span data-stu-id="7787d-218">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "sequenceNumber": 10,
      "subscriptionId":"{subscription_guid}",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@{tenant_guid}/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@{tenant_guid}/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"{long_id_string}"
      }
    }
  ]
}
```

### <a name="processing-the-change-notification"></a><span data-ttu-id="7787d-219">Processando a notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="7787d-219">Processing the change notification</span></span>

<span data-ttu-id="7787d-220">Seu processo deve processar todas as notificações de alteração recebidas.</span><span class="sxs-lookup"><span data-stu-id="7787d-220">Your process should process every change notification it receives.</span></span> <span data-ttu-id="7787d-221">Veja a seguir as tarefas mínimas que seu aplicativo deve executar para processar uma notificação de alteração:</span><span class="sxs-lookup"><span data-stu-id="7787d-221">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="7787d-222">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-222">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="7787d-223">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará publicar a notificação de alteração diversas vezes, por um período de cerca de 4 horas; Após isso, a notificação de alteração será cancelada e não será entregue.</span><span class="sxs-lookup"><span data-stu-id="7787d-223">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="7787d-224">**Observação:** Envie um `202 - Accepted` código de status assim que receber a notificação de alteração, mesmo antes de validar sua autenticidade.</span><span class="sxs-lookup"><span data-stu-id="7787d-224">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="7787d-225">Você está apenas confirmando o recebimento da notificação de alteração e evitando tentativas desnecessárias.</span><span class="sxs-lookup"><span data-stu-id="7787d-225">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="7787d-226">O tempo limite atual é de 30 segundos, mas pode ser reduzido no futuro para otimizar o desempenho do serviço.</span><span class="sxs-lookup"><span data-stu-id="7787d-226">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="7787d-227">Se a URL de notificação não responder dentro de 30 segundos para mais de 10% das solicitações do Microsoft Graph em um período de 10 minutos, todas as notificações a seguir serão atrasadas e repetidas por um período de 4 horas.</span><span class="sxs-lookup"><span data-stu-id="7787d-227">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="7787d-228">Se uma URL de notificação não responder dentro de 30 segundos por mais de 20% das solicitações do Microsoft Graph em um período de 10 minutos, todas as notificações a seguir serão descartadas.</span><span class="sxs-lookup"><span data-stu-id="7787d-228">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="7787d-229">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="7787d-229">Validate the `clientState` property.</span></span> <span data-ttu-id="7787d-230">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7787d-230">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="7787d-231">**Observação:** Se isso não for verdadeiro, você não deve considerar essa uma notificação de alteração válida.</span><span class="sxs-lookup"><span data-stu-id="7787d-231">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="7787d-232">É possível que a notificação de alteração não tenha origem no Microsoft Graph e tenha sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="7787d-232">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="7787d-233">Você também deve investigar onde a notificação de alteração provém e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="7787d-233">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="7787d-234">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="7787d-234">Update your application based on your business logic.</span></span>

<span data-ttu-id="7787d-235">Repita para outras notificações de alteração na solicitação.</span><span class="sxs-lookup"><span data-stu-id="7787d-235">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="7787d-236">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="7787d-236">Code samples</span></span>

<span data-ttu-id="7787d-237">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="7787d-237">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="7787d-238">Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7787d-238">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="7787d-239">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="7787d-239">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="7787d-240">Exemplo de Webhooks do Microsoft Graph para o ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="7787d-240">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="7787d-241">Exemplo de Webhooks do Microsoft Graph para Java Spring</span><span class="sxs-lookup"><span data-stu-id="7787d-241">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="7787d-242">Configuração do firewall</span><span class="sxs-lookup"><span data-stu-id="7787d-242">Firewall configuration</span></span>

<span data-ttu-id="7787d-243">Opcionalmente, você pode configurar o firewall que protege a URL de notificação para permitir conexões de entrada somente pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7787d-243">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="7787d-244">Isso permite que você reduza mais exposição a notificações de alteração inválidas que são enviadas para sua URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="7787d-244">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="7787d-245">Essas notificações de alteração inválidas podem estar tentando disparar a lógica personalizada que você implementou.</span><span class="sxs-lookup"><span data-stu-id="7787d-245">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="7787d-246">Para obter uma lista completa de endereços IP usados pelo Microsoft Graph para fornecer notificações de alteração, consulte [pontos de extremidade adicionais para o microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span><span class="sxs-lookup"><span data-stu-id="7787d-246">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="7787d-247">**Observação:** Os endereços IP listados que são usados para fornecer notificações de alteração podem ser atualizados a qualquer momento sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="7787d-247">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="see-also"></a><span data-ttu-id="7787d-248">Confira também</span><span class="sxs-lookup"><span data-stu-id="7787d-248">See also</span></span>

- [<span data-ttu-id="7787d-249">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-249">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="7787d-250">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-250">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="7787d-251">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="7787d-251">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="7787d-252">tipo de recurso [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="7787d-252">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="7787d-253">tipo de recurso [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="7787d-253">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="7787d-254">Tutorial de controle de alterações e notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="7787d-254">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="7787d-255">Notificações do ciclo de vida (visualização)</span><span class="sxs-lookup"><span data-stu-id="7787d-255">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

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
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage

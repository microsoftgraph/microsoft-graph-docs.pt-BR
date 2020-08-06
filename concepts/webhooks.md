---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações de alteração para atualizar seu estado após alterações.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 155d09ee373b52307fe4f22fbedee21ee40632d8
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567226"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="09d5d-105">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="09d5d-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="09d5d-p102">A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações de alteração para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="09d5d-p102">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="09d5d-109">Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações de alteração por push para a URL especificada na assinatura.</span><span class="sxs-lookup"><span data-stu-id="09d5d-109">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="09d5d-110">O aplicativo então realiza ações de acordo com sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="09d5d-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="09d5d-111">Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.</span><span class="sxs-lookup"><span data-stu-id="09d5d-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="09d5d-112">Tutorial: usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="09d5d-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="09d5d-113">Por padrão, as notificações de alteração não contêm dados de recursos, exceto o `id`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="09d5d-114">Se o aplicativo exigir dados de recursos, ele poderá fazer chamadas para as APIs do Microsoft Graph para obter o recurso completo.</span><span class="sxs-lookup"><span data-stu-id="09d5d-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="09d5d-115">Este artigo usa o recurso de **usuário** como um exemplo para trabalhar com notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="09d5d-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="09d5d-116">Um aplicativo também pode se inscrever para alterar notificações que incluem dados de recursos, para evitar a necessidade de fazer chamadas de API adicionais para acessar os dados.</span><span class="sxs-lookup"><span data-stu-id="09d5d-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additional API calls to access the data.</span></span> <span data-ttu-id="09d5d-117">Esses aplicativos precisarão implementar um código extra para lidar com os requisitos de tais notificações, especificamente: responder às notificações do ciclo de vida da assinatura, validar a autenticidade das notificações e descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="09d5d-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="09d5d-118">Mais tipos de recursos terão suporte para esse tipo de notificações no futuro.</span><span class="sxs-lookup"><span data-stu-id="09d5d-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="09d5d-119">Para saber mais sobre como trabalhar com essas notificações, confira [Configurar notificações de alteração que incluem dados de recurso (visualização)](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="09d5d-119">For details about how to work with these notifications, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="09d5d-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="09d5d-120">Supported resources</span></span>

<span data-ttu-id="09d5d-121">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="09d5d-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="09d5d-122">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="09d5d-122">Outlook [message][]</span></span>
- <span data-ttu-id="09d5d-123">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="09d5d-123">Outlook [event][]</span></span>
- <span data-ttu-id="09d5d-124">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="09d5d-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="09d5d-125">[list][]</span><span class="sxs-lookup"><span data-stu-id="09d5d-125">[list][]</span></span>
- <span data-ttu-id="09d5d-126">[user][]</span><span class="sxs-lookup"><span data-stu-id="09d5d-126">[user][]</span></span>
- <span data-ttu-id="09d5d-127">[group][]</span><span class="sxs-lookup"><span data-stu-id="09d5d-127">[group][]</span></span>
- <span data-ttu-id="09d5d-128">[Conversa][] em grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="09d5d-128">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="09d5d-129">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="09d5d-129">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="09d5d-130">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="09d5d-130">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="09d5d-131">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="09d5d-131">Security [alert][]</span></span>
- <span data-ttu-id="09d5d-132">[callRecord][] do Teams</span><span class="sxs-lookup"><span data-stu-id="09d5d-132">Teams [callRecord][]</span></span>
- <span data-ttu-id="09d5d-133">[chatMessage][] do Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="09d5d-133">Teams [chatMessage][] (preview)</span></span>
- <span data-ttu-id="09d5d-134">[presence][] do Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="09d5d-134">Teams [presence][] (preview)</span></span>

<span data-ttu-id="09d5d-135">Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="09d5d-135">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="09d5d-136">Ou para um recurso de nível superior: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="09d5d-136">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span></span>

<span data-ttu-id="09d5d-137">Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="09d5d-137">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span></span>

<span data-ttu-id="09d5d-138">Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="09d5d-138">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="09d5d-139">Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="09d5d-139">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="09d5d-140">Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="09d5d-140">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="09d5d-141">Limitações de recursos do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="09d5d-141">Azure AD resource limitations</span></span>

<span data-ttu-id="09d5d-142">Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:</span><span class="sxs-lookup"><span data-stu-id="09d5d-142">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="09d5d-143">**Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09d5d-143">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="09d5d-144">Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="09d5d-144">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="09d5d-145">Cotas máximas de assinaturas:</span><span class="sxs-lookup"><span data-stu-id="09d5d-145">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="09d5d-146">Por aplicativo (para todos os locatários combinados): 50.000 assinaturas totais</span><span class="sxs-lookup"><span data-stu-id="09d5d-146">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="09d5d-147">Por locatário (para todos os aplicativos combinados): 1000 total de assinaturas em todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="09d5d-147">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="09d5d-148">Combinação por aplicativo e locatário: 100 assinaturas no total</span><span class="sxs-lookup"><span data-stu-id="09d5d-148">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="09d5d-149">Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-149">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="09d5d-150">A propriedade `message` explicará qual limite foi excedido.</span><span class="sxs-lookup"><span data-stu-id="09d5d-150">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="09d5d-151">Não há suporte a locatários do Microsoft Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="09d5d-151">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="09d5d-152">Não há suporte a notificações de alteração para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="09d5d-152">Change notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="09d5d-153">Existe um [problema conhecido](known-issues.md#change-notifications) nas assinaturas de usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="09d5d-153">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="09d5d-154">Limitações de recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="09d5d-154">Outlook resource limitations</span></span>

<span data-ttu-id="09d5d-155">Ao se inscrever em recursos do Outlook, tais como **mensagens**, **eventos** ou **contatos**, se você decidir usar o *nome UPN* em um caminho de recurso, a solicitação de assinatura pode falhar caso o UPN contenha um apóstrofo.</span><span class="sxs-lookup"><span data-stu-id="09d5d-155">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="09d5d-156">Considere usar IDs de usuário de GUID em vez de UPNs para evitar esse problema.</span><span class="sxs-lookup"><span data-stu-id="09d5d-156">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="09d5d-157">Por exemplo, em vez de usar o caminho de recursos:</span><span class="sxs-lookup"><span data-stu-id="09d5d-157">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="09d5d-158">Use:</span><span class="sxs-lookup"><span data-stu-id="09d5d-158">Use:</span></span> 

`/users/{guid-user-id}/messages`

### <a name="teams-resource-limitations-preview"></a><span data-ttu-id="09d5d-159">Limitações de recursos do Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="09d5d-159">Teams resource limitations (preview)</span></span>

<span data-ttu-id="09d5d-160">É permitida uma única assinatura ativa por canal ou chat por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="09d5d-160">A single active subscription per channel or chat per application is allowed.</span></span>

<span data-ttu-id="09d5d-161">É permitido um máximo de 10000 assinaturas ativas por organização em chats e canais para todos os aplicativos.</span><span class="sxs-lookup"><span data-stu-id="09d5d-161">A maximum of 10000 active subscriptions per organization on chats and channels for all applications is allowed.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="09d5d-162">Tempo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-162">Subscription lifetime</span></span>

<span data-ttu-id="09d5d-163">As assinaturas têm tempo de vida limitado.</span><span class="sxs-lookup"><span data-stu-id="09d5d-163">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="09d5d-164">Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="09d5d-164">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="09d5d-165">Caso contrário, será preciso criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="09d5d-165">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="09d5d-166">Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="09d5d-166">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="09d5d-167">Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="09d5d-167">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="09d5d-168">Gerenciar assinaturas</span><span class="sxs-lookup"><span data-stu-id="09d5d-168">Managing subscriptions</span></span>

<span data-ttu-id="09d5d-169">Os clientes podem criar, renovar e excluir assinaturas.</span><span class="sxs-lookup"><span data-stu-id="09d5d-169">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="09d5d-170">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-170">Creating a subscription</span></span>

<span data-ttu-id="09d5d-171">Criar uma assinatura é a primeira etapa para começar a receber notificações de alteração de um recurso.</span><span class="sxs-lookup"><span data-stu-id="09d5d-171">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="09d5d-172">O processo de assinatura ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="09d5d-172">The subscription process is as follows:</span></span>

1. <span data-ttu-id="09d5d-173">O cliente envia uma solicitação de assinatura (POST) para um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="09d5d-173">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="09d5d-174">O Microsoft Graph verifica a solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-174">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="09d5d-175">Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-175">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="09d5d-176">Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.</span><span class="sxs-lookup"><span data-stu-id="09d5d-176">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="09d5d-177">O cliente envia o token de validação de volta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="09d5d-177">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="09d5d-178">O Microsoft Graph envia uma resposta de volta para o cliente.</span><span class="sxs-lookup"><span data-stu-id="09d5d-178">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="09d5d-179">O cliente deve armazenar a ID da assinatura para correlacionar notificações de alteração com a assinatura.</span><span class="sxs-lookup"><span data-stu-id="09d5d-179">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="09d5d-180">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-180">Subscription request example</span></span>

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

<span data-ttu-id="09d5d-181">As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="09d5d-181">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="09d5d-182">Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="09d5d-182">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="09d5d-183">A propriedade `resource` especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="09d5d-183">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="09d5d-184">Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-184">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="09d5d-185">Embora `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="09d5d-185">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="09d5d-186">A definição desta propriedade permitirá confirmar se as notificações de alteração recebidas partiram do serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="09d5d-186">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="09d5d-187">Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="09d5d-187">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="09d5d-188">Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="09d5d-188">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

> <span data-ttu-id="09d5d-189">**Observação:** todos os parâmetros de cadeia de caracteres de consulta incluídos na propriedade `notificationUrl` serão incluídos na solicitação de POST HTTP quando as notificações estiverem sendo entregues.</span><span class="sxs-lookup"><span data-stu-id="09d5d-189">**Note:** any query string parameter included in the `notificationUrl` property will be included in the HTTP POST request when notifications are being delivered.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="09d5d-190">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="09d5d-190">Notification endpoint validation</span></span>

<span data-ttu-id="09d5d-191">O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="09d5d-191">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="09d5d-192">O processo de validação ocorre da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="09d5d-192">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="09d5d-193">O Microsoft Graph codifica um token de validação e o inclui em uma solicitação POST na URL da notificação:</span><span class="sxs-lookup"><span data-stu-id="09d5d-193">Microsoft Graph encodes a validation token and includes it in a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

1. <span data-ttu-id="09d5d-194">O cliente deve decodificar corretamente o `validationToken` fornecido na etapa anterior e escapar de um HTML/JavaScript.</span><span class="sxs-lookup"><span data-stu-id="09d5d-194">The client must properly decode the `validationToken` provided in the preceding step, and escape any HTML/JavaScript.</span></span>

   <span data-ttu-id="09d5d-195">Escapar é uma boa prática porque atores maliciosos podem usar o ponto de extremidade de notificação para o tipo de ataques de script entre sites.</span><span class="sxs-lookup"><span data-stu-id="09d5d-195">Escaping is a good practice because malicious actors can use the notification endpoint for cross-site scripting type of attacks.</span></span>

   <span data-ttu-id="09d5d-196">Em geral, trate o valor do token de validação como opaco, uma vez que o formato do token geralmente pode ser alterado sem aviso.</span><span class="sxs-lookup"><span data-stu-id="09d5d-196">In general, treat the validation token value as opaque, as the token format can generally change without notice.</span></span> <span data-ttu-id="09d5d-197">O Microsoft Graph nunca envia nenhum valor contendo código HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="09d5d-197">Microsoft Graph never sends any value containing HTML or JavaScript code.</span></span>

1. <span data-ttu-id="09d5d-198">O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos da etapa 1:</span><span class="sxs-lookup"><span data-stu-id="09d5d-198">The client must provide a response with the following characteristics within 10 seconds of step 1:</span></span>

    - <span data-ttu-id="09d5d-199">Um código de status de `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-199">A status code of `HTTP 200 OK`.</span></span>
    - <span data-ttu-id="09d5d-200">Um tipo de conteúdo de `text/plain`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-200">A content type of `text/plain`.</span></span>
    - <span data-ttu-id="09d5d-201">Um corpo que inclui o token de validação _decodificado_.</span><span class="sxs-lookup"><span data-stu-id="09d5d-201">A body that includes the _decoded_ validation token.</span></span>

    <span data-ttu-id="09d5d-202">O cliente deve descartar o token de validação depois de o fornecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="09d5d-202">The client should discard the validation token after providing it in the response.</span></span>

    > <span data-ttu-id="09d5d-203">**Importante:** se o cliente retornar um token de validação codificado, a validação falhará.</span><span class="sxs-lookup"><span data-stu-id="09d5d-203">**Important:** If the client returns an encoded validation token, the validation will fail.</span></span>

<span data-ttu-id="09d5d-204">Além disso, você pode usar a [coleção do Microsoft Graph Postman](use-postman.md) para confirmar que o ponto de extremidade implementa a solicitação de validação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-204">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="09d5d-205">A solicitação de **Validação de Assinaturas** na pasta **Diversos** fornece testes de unidade que validam a resposta fornecida por seu ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="09d5d-205">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![resultados do teste de resposta de validação](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="09d5d-207">Renovar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-207">Renewing a subscription</span></span>

<span data-ttu-id="09d5d-208">O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-208">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="09d5d-209">A propriedade `expirationDateTime` é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="09d5d-209">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="09d5d-210">Exemplo de renovação de assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-210">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="09d5d-211">Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.</span><span class="sxs-lookup"><span data-stu-id="09d5d-211">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="09d5d-212">O objeto subscription inclui o novo valor de `expirationDateTime`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-212">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="09d5d-213">Excluindo uma assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-213">Deleting a subscription</span></span>

<span data-ttu-id="09d5d-214">O cliente pode parar de receber notificações de alteração excluindo a assinatura com o uso de sua ID.</span><span class="sxs-lookup"><span data-stu-id="09d5d-214">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="09d5d-215">Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-215">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="09d5d-216">Notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="09d5d-216">Change notifications</span></span>

<span data-ttu-id="09d5d-217">Com uma assinatura do cliente em um recurso, o Microsoft Graph envia uma solicitação `POST` para a URL da notificação sempre que o recurso é alterado.</span><span class="sxs-lookup"><span data-stu-id="09d5d-217">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="09d5d-218">Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-218">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="09d5d-219">**Observação:** se um cliente tiver várias assinaturas que monitoram o mesmo recurso e usam a mesma URL de notificação, o Microsoft Graph poderá enviar várias notificações de alteração que correspondam a diferentes assinaturas, cada uma mostrando a ID da assinatura correspondente.</span><span class="sxs-lookup"><span data-stu-id="09d5d-219">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="09d5d-220">Não há garantias de que todas as notificações na solicitação `POST` pertencerão a uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="09d5d-220">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="09d5d-221">Exemplo de notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="09d5d-221">Change notification example</span></span>

<span data-ttu-id="09d5d-222">Esta seção mostra um exemplo de uma notificação para a criação de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="09d5d-222">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="09d5d-223">Quando o usuário recebe um email, o Microsoft Graph envia uma notificação de alteração como mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="09d5d-223">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="09d5d-224">Observe que a notificação está em uma coleção representada no campo `value`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-224">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="09d5d-225">Confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection) para obter detalhes da carga de notificação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-225">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="09d5d-226">Quando várias alterações ocorrerem, o Microsoft Graph poderá enviar várias notificações que correspondam a diferentes assinaturas na mesma solicitação `POST`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-226">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
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

### <a name="processing-the-change-notification"></a><span data-ttu-id="09d5d-227">Processar a notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="09d5d-227">Processing the change notification</span></span>

<span data-ttu-id="09d5d-228">O processo deve processar todas as notificações de alteração recebidas.</span><span class="sxs-lookup"><span data-stu-id="09d5d-228">Your process should process every change notification it receives.</span></span> <span data-ttu-id="09d5d-229">Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação de alteração:</span><span class="sxs-lookup"><span data-stu-id="09d5d-229">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="09d5d-230">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="09d5d-230">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="09d5d-231">Se o Microsoft Graph não receber um código de classe 2xx, ele tentará publicar a notificação de alteração algumas vezes, por um período de aproximadamente 4 horas; depois disso, a notificação será descartada e não será entregue.</span><span class="sxs-lookup"><span data-stu-id="09d5d-231">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="09d5d-232">**Observação:** Envie um código de status `202 - Accepted` assim que receber a notificação de alteração, mesmo antes de validar a sua autenticidade.</span><span class="sxs-lookup"><span data-stu-id="09d5d-232">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="09d5d-233">Você está simplesmente confirmando o recebimento da notificação de alteração e impedindo tentativas desnecessárias.</span><span class="sxs-lookup"><span data-stu-id="09d5d-233">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="09d5d-234">O tempo limite atual é de 30 segundos, mas pode ser reduzido no futuro para otimizar o desempenho do serviço.</span><span class="sxs-lookup"><span data-stu-id="09d5d-234">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="09d5d-235">Se a URL da notificação não responder dentro de 30 segundos para mais de 10% das solicitações do Microsoft Graph durante um período de 10 minutos, todas as notificações a seguir serão adiadas e repetidas por um período de 4 horas.</span><span class="sxs-lookup"><span data-stu-id="09d5d-235">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="09d5d-236">Se uma URL da notificação não responder dentro de 30 segundos para mais de 20% das solicitações do Microsoft Graph durante um período de 10 minutos, todas as notificações a seguir serão descartadas.</span><span class="sxs-lookup"><span data-stu-id="09d5d-236">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="09d5d-237">Validar a propriedade `clientState`.</span><span class="sxs-lookup"><span data-stu-id="09d5d-237">Validate the `clientState` property.</span></span> <span data-ttu-id="09d5d-238">Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="09d5d-238">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="09d5d-239">**Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida.</span><span class="sxs-lookup"><span data-stu-id="09d5d-239">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="09d5d-240">É possível que a notificação de alteração não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor.</span><span class="sxs-lookup"><span data-stu-id="09d5d-240">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="09d5d-241">Você também deve investigar de onde vem a notificação de alteração e tomar as medidas apropriadas.</span><span class="sxs-lookup"><span data-stu-id="09d5d-241">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="09d5d-242">Atualize seu aplicativo com base na sua lógica comercial.</span><span class="sxs-lookup"><span data-stu-id="09d5d-242">Update your application based on your business logic.</span></span>

<span data-ttu-id="09d5d-243">Repita o procedimento para outras notificações de alteração na solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-243">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="09d5d-244">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="09d5d-244">Code samples</span></span>

<span data-ttu-id="09d5d-245">Os exemplos de código a seguir estão disponíveis no GitHub.</span><span class="sxs-lookup"><span data-stu-id="09d5d-245">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="09d5d-246">Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="09d5d-246">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="09d5d-247">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="09d5d-247">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="09d5d-248">Exemplo de Webhooks do Microsoft Graph para o ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="09d5d-248">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="09d5d-249">Exemplo de Webhooks do Microsoft Graph para Java Spring</span><span class="sxs-lookup"><span data-stu-id="09d5d-249">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="09d5d-250">Configuração do firewall</span><span class="sxs-lookup"><span data-stu-id="09d5d-250">Firewall configuration</span></span>

<span data-ttu-id="09d5d-251">Opcionalmente, você pode configurar o firewall que protege a URL de notificação para permitir conexões de entrada somente pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="09d5d-251">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="09d5d-252">Isso permite que você reduza ainda mais a exposição a notificações de alteração inválidas que são enviadas para sua URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="09d5d-252">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="09d5d-253">Essas notificações de alteração inválidas podem estar tentando desencadear a lógica personalizada que você implementou.</span><span class="sxs-lookup"><span data-stu-id="09d5d-253">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="09d5d-254">Para obter uma lista completa de endereços IP usados pelo Microsoft Graph para oferecer notificações de alteração, confira [pontos de extremidade adicionais para Microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span><span class="sxs-lookup"><span data-stu-id="09d5d-254">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="09d5d-255">**Observação:** Os endereços IP listados que são usados para fornecer notificações de alteração podem ser atualizados a qualquer momento sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="09d5d-255">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="see-also"></a><span data-ttu-id="09d5d-256">Confira também</span><span class="sxs-lookup"><span data-stu-id="09d5d-256">See also</span></span>

- [<span data-ttu-id="09d5d-257">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-257">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="09d5d-258">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-258">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="09d5d-259">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="09d5d-259">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="09d5d-260">Tipo de recurso [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="09d5d-260">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="09d5d-261">Tipo de recurso [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="09d5d-261">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="09d5d-262">Tutorial para notificações de alteração as notificações e controle de alterações</span><span class="sxs-lookup"><span data-stu-id="09d5d-262">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="09d5d-263">Notificações do ciclo de vida (visualização)</span><span class="sxs-lookup"><span data-stu-id="09d5d-263">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

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
[presence]: /graph/api/resources/presence
[chatMessage]: /graph/api/resources/chatmessage
[list]: /graph/api/resources/list

---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: piotrci
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 70af093b6ed782ba7bf447c339e5187439849970
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844264"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="04d2c-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="04d2c-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d2c-105">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04d2c-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="04d2c-106">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="04d2c-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="04d2c-107">Um [alerta][] da API de Segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="04d2c-107">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="04d2c-108">Um [chat][] enviado por meio de equipes ou canais no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="04d2c-108">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="04d2c-109">Uma [conversa][] em um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="04d2c-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="04d2c-110">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="04d2c-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="04d2c-111">Um [mensagem][], [evento][], ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="04d2c-111">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="04d2c-112">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="04d2c-112">A [user][] or [group][] in Azure Active Directory</span></span>

## <a name="methods"></a><span data-ttu-id="04d2c-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="04d2c-113">Methods</span></span>

| <span data-ttu-id="04d2c-114">Método</span><span class="sxs-lookup"><span data-stu-id="04d2c-114">Method</span></span> | <span data-ttu-id="04d2c-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="04d2c-115">Return Type</span></span> | <span data-ttu-id="04d2c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="04d2c-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="04d2c-117">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="04d2c-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="04d2c-118">subscription</span><span class="sxs-lookup"><span data-stu-id="04d2c-118">subscription</span></span>](subscription.md) | <span data-ttu-id="04d2c-119">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="04d2c-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="04d2c-120">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="04d2c-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="04d2c-121">subscription</span><span class="sxs-lookup"><span data-stu-id="04d2c-121">subscription</span></span>](subscription.md) | <span data-ttu-id="04d2c-122">Renovar uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="04d2c-122">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="04d2c-123">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="04d2c-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="04d2c-124">assinatura</span><span class="sxs-lookup"><span data-stu-id="04d2c-124">subscription</span></span>](subscription.md) | <span data-ttu-id="04d2c-125">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="04d2c-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="04d2c-126">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="04d2c-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="04d2c-127">subscription</span><span class="sxs-lookup"><span data-stu-id="04d2c-127">subscription</span></span>](subscription.md) | <span data-ttu-id="04d2c-128">Leia as propriedades e as relações do objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="04d2c-128">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="04d2c-129">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="04d2c-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="04d2c-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="04d2c-130">None</span></span> | <span data-ttu-id="04d2c-131">Excluir um objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="04d2c-131">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="04d2c-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04d2c-132">Properties</span></span>

| <span data-ttu-id="04d2c-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04d2c-133">Property</span></span> | <span data-ttu-id="04d2c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="04d2c-134">Type</span></span> | <span data-ttu-id="04d2c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="04d2c-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="04d2c-136">changeType</span><span class="sxs-lookup"><span data-stu-id="04d2c-136">changeType</span></span> | <span data-ttu-id="04d2c-137">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-137">string</span></span> | <span data-ttu-id="04d2c-138">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="04d2c-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="04d2c-139">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="04d2c-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="04d2c-140">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="04d2c-140">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="04d2c-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d2c-141">Required.</span></span> <br><br><span data-ttu-id="04d2c-142">Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="04d2c-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="04d2c-143">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="04d2c-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="04d2c-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="04d2c-144">notificationUrl</span></span> | <span data-ttu-id="04d2c-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04d2c-145">string</span></span> | <span data-ttu-id="04d2c-146">A URL do ponto de extremidade que recebe as notificações.</span><span class="sxs-lookup"><span data-stu-id="04d2c-146">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="04d2c-147">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="04d2c-147">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="04d2c-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d2c-148">Required.</span></span> |
| <span data-ttu-id="04d2c-149">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="04d2c-149">lifecycleNotificationUrl</span></span> | <span data-ttu-id="04d2c-150">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-150">string</span></span> | <span data-ttu-id="04d2c-151">A URL do ponto de extremidade que recebe notificações de ciclo `subscriptionRemoved` de `missed` vida, incluindo e notificações.</span><span class="sxs-lookup"><span data-stu-id="04d2c-151">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="04d2c-152">Se não for fornecido, as notificações serão entregues ao **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="04d2c-152">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="04d2c-153">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="04d2c-153">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="04d2c-154">Opcional.</span><span class="sxs-lookup"><span data-stu-id="04d2c-154">Optional.</span></span> <br><br><span data-ttu-id="04d2c-155">[Leia mais](/graph/webhooks-outlook-authz) sobre como os recursos do Outlook usam notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="04d2c-155">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="04d2c-156">recurso</span><span class="sxs-lookup"><span data-stu-id="04d2c-156">resource</span></span> | <span data-ttu-id="04d2c-157">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-157">string</span></span> | <span data-ttu-id="04d2c-158">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="04d2c-158">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="04d2c-159">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="04d2c-159">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="04d2c-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d2c-160">Required.</span></span> |
| <span data-ttu-id="04d2c-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="04d2c-161">expirationDateTime</span></span> | <span data-ttu-id="04d2c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04d2c-162">DateTimeOffset</span></span> | <span data-ttu-id="04d2c-163">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="04d2c-163">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="04d2c-164">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="04d2c-164">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="04d2c-165">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="04d2c-165">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="04d2c-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d2c-166">Required.</span></span> |
| <span data-ttu-id="04d2c-167">clientState</span><span class="sxs-lookup"><span data-stu-id="04d2c-167">clientState</span></span> | <span data-ttu-id="04d2c-168">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-168">string</span></span> | <span data-ttu-id="04d2c-169">Especifica o valor da propriedade **ClientState** enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="04d2c-169">Specifies the value of the **clientState** property sent by the service in each notification.</span></span> <span data-ttu-id="04d2c-170">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="04d2c-170">The maximum length is 255 characters.</span></span> <span data-ttu-id="04d2c-171">O cliente pode verificar se a notificação veio do serviço, comparando o valor da propriedade **ClientState** enviada com a assinatura com o valor da propriedade **ClientState** recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="04d2c-171">The client can check that the notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each notification.</span></span> <span data-ttu-id="04d2c-172">Opcional.</span><span class="sxs-lookup"><span data-stu-id="04d2c-172">Optional.</span></span> |
| <span data-ttu-id="04d2c-173">id</span><span class="sxs-lookup"><span data-stu-id="04d2c-173">id</span></span> | <span data-ttu-id="04d2c-174">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-174">string</span></span> | <span data-ttu-id="04d2c-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04d2c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="04d2c-177">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="04d2c-177">applicationId</span></span> | <span data-ttu-id="04d2c-178">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-178">string</span></span> | <span data-ttu-id="04d2c-179">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="04d2c-179">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="04d2c-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04d2c-180">Read-only.</span></span> |
| <span data-ttu-id="04d2c-181">creatorId</span><span class="sxs-lookup"><span data-stu-id="04d2c-181">creatorId</span></span> | <span data-ttu-id="04d2c-182">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04d2c-182">string</span></span> | <span data-ttu-id="04d2c-183">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="04d2c-183">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="04d2c-184">Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de.</span><span class="sxs-lookup"><span data-stu-id="04d2c-184">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="04d2c-185">Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d2c-185">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="04d2c-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04d2c-186">Read-only.</span></span> |
| <span data-ttu-id="04d2c-187">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="04d2c-187">includeResourceData</span></span> | <span data-ttu-id="04d2c-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="04d2c-188">Boolean</span></span> | <span data-ttu-id="04d2c-189">Quando definido como `true`, as notificações de alteração [incluem dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de chat).</span><span class="sxs-lookup"><span data-stu-id="04d2c-189">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="04d2c-190">Opcional.</span><span class="sxs-lookup"><span data-stu-id="04d2c-190">Optional.</span></span> | 
| <span data-ttu-id="04d2c-191">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="04d2c-191">encryptionCertificate</span></span> | <span data-ttu-id="04d2c-192">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-192">string</span></span> | <span data-ttu-id="04d2c-193">Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar dados de recurso em notificações.</span><span class="sxs-lookup"><span data-stu-id="04d2c-193">A base64-encoded representation of a certificate with a public key used to encrypt resource data in notifications.</span></span> <span data-ttu-id="04d2c-194">Opcional.</span><span class="sxs-lookup"><span data-stu-id="04d2c-194">Optional.</span></span> <span data-ttu-id="04d2c-195">Obrigatório quando **includeResourceData** é true.</span><span class="sxs-lookup"><span data-stu-id="04d2c-195">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="04d2c-196">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="04d2c-196">encryptionCertificateId</span></span> | <span data-ttu-id="04d2c-197">string</span><span class="sxs-lookup"><span data-stu-id="04d2c-197">string</span></span> | <span data-ttu-id="04d2c-198">Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar dados de recurso.</span><span class="sxs-lookup"><span data-stu-id="04d2c-198">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="04d2c-199">Opcional.</span><span class="sxs-lookup"><span data-stu-id="04d2c-199">Optional.</span></span> <span data-ttu-id="04d2c-200">Obrigatório quando **includeResourceData** é true.</span><span class="sxs-lookup"><span data-stu-id="04d2c-200">Required when **includeResourceData** is true.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="04d2c-201">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="04d2c-201">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="04d2c-202">Recurso</span><span class="sxs-lookup"><span data-stu-id="04d2c-202">Resource</span></span>            | <span data-ttu-id="04d2c-203">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="04d2c-203">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="04d2c-204">**Alerta** de segurança</span><span class="sxs-lookup"><span data-stu-id="04d2c-204">Security **alert**</span></span>     | <span data-ttu-id="04d2c-205">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="04d2c-205">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="04d2c-206">Teams **chat**</span><span class="sxs-lookup"><span data-stu-id="04d2c-206">Teams **chatMessage**</span></span>    | <span data-ttu-id="04d2c-207">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="04d2c-207">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="04d2c-208">**Conversa** de grupo</span><span class="sxs-lookup"><span data-stu-id="04d2c-208">Group **conversation**</span></span> | <span data-ttu-id="04d2c-209">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="04d2c-209">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="04d2c-210">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="04d2c-210">OneDrive **driveItem**</span></span>    | <span data-ttu-id="04d2c-211">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="04d2c-211">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="04d2c-212">**Mensagem**, **evento**, **contato** do Outlook</span><span class="sxs-lookup"><span data-stu-id="04d2c-212">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="04d2c-213">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="04d2c-213">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="04d2c-214">**usuário**, **grupo**, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="04d2c-214">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="04d2c-215">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="04d2c-215">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="04d2c-216">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="04d2c-216">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="04d2c-217">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="04d2c-217">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="04d2c-218">Relações</span><span class="sxs-lookup"><span data-stu-id="04d2c-218">Relationships</span></span>

<span data-ttu-id="04d2c-219">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04d2c-219">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04d2c-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04d2c-220">JSON representation</span></span>

<span data-ttu-id="04d2c-221">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04d2c-221">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string"
}
```

[contato]: ./contact.md
[contact]: ./contact.md
[conversa]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[chatMessage]: ./chatmessage.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

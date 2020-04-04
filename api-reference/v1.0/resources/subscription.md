---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8ede2274abebbba1148762f5d3606cd61a4578a4
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108428"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="08fd2-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="08fd2-104">subscription resource type</span></span>

<span data-ttu-id="08fd2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08fd2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08fd2-106">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="08fd2-106">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="08fd2-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="08fd2-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="08fd2-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="08fd2-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="08fd2-109">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="08fd2-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="08fd2-110">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="08fd2-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="08fd2-111">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="08fd2-111">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="08fd2-112">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="08fd2-112">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="08fd2-113">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="08fd2-113">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="08fd2-114">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="08fd2-114">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="08fd2-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="08fd2-115">Methods</span></span>

| <span data-ttu-id="08fd2-116">Método</span><span class="sxs-lookup"><span data-stu-id="08fd2-116">Method</span></span> | <span data-ttu-id="08fd2-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08fd2-117">Return Type</span></span> | <span data-ttu-id="08fd2-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="08fd2-118">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="08fd2-119">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="08fd2-119">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="08fd2-120">subscription</span><span class="sxs-lookup"><span data-stu-id="08fd2-120">subscription</span></span>](subscription.md) | <span data-ttu-id="08fd2-121">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="08fd2-121">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="08fd2-122">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="08fd2-122">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="08fd2-123">subscription</span><span class="sxs-lookup"><span data-stu-id="08fd2-123">subscription</span></span>](subscription.md) | <span data-ttu-id="08fd2-124">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="08fd2-124">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="08fd2-125">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="08fd2-125">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="08fd2-126">assinatura</span><span class="sxs-lookup"><span data-stu-id="08fd2-126">subscription</span></span>](subscription.md) | <span data-ttu-id="08fd2-127">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="08fd2-127">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="08fd2-128">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="08fd2-128">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="08fd2-129">subscription</span><span class="sxs-lookup"><span data-stu-id="08fd2-129">subscription</span></span>](subscription.md) | <span data-ttu-id="08fd2-130">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="08fd2-130">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="08fd2-131">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="08fd2-131">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="08fd2-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="08fd2-132">None</span></span> | <span data-ttu-id="08fd2-133">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-133">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="08fd2-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08fd2-134">Properties</span></span>

| <span data-ttu-id="08fd2-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08fd2-135">Property</span></span> | <span data-ttu-id="08fd2-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="08fd2-136">Type</span></span> | <span data-ttu-id="08fd2-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="08fd2-137">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="08fd2-138">changeType</span><span class="sxs-lookup"><span data-stu-id="08fd2-138">changeType</span></span> | <span data-ttu-id="08fd2-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08fd2-139">string</span></span> | <span data-ttu-id="08fd2-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08fd2-140">Required.</span></span> <span data-ttu-id="08fd2-141">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="08fd2-141">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="08fd2-142">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="08fd2-142">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="08fd2-143">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="08fd2-143">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="08fd2-144">Observação: As notificações de lista e do item na raiz da unidade têm suporte apenas para o changeType `updated`.</span><span class="sxs-lookup"><span data-stu-id="08fd2-144">Note: Drive root item and list notifications support only the `updated` changeType.</span></span> <span data-ttu-id="08fd2-145">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="08fd2-145">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="08fd2-146">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="08fd2-146">notificationUrl</span></span> | <span data-ttu-id="08fd2-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08fd2-147">string</span></span> | <span data-ttu-id="08fd2-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08fd2-148">Required.</span></span> <span data-ttu-id="08fd2-149">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="08fd2-149">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="08fd2-150">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="08fd2-150">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="08fd2-151">recurso</span><span class="sxs-lookup"><span data-stu-id="08fd2-151">resource</span></span> | <span data-ttu-id="08fd2-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08fd2-152">string</span></span> | <span data-ttu-id="08fd2-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08fd2-153">Required.</span></span> <span data-ttu-id="08fd2-154">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="08fd2-154">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="08fd2-155">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="08fd2-155">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="08fd2-156">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="08fd2-156">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="08fd2-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="08fd2-157">expirationDateTime</span></span> | [<span data-ttu-id="08fd2-158">dateTime</span><span class="sxs-lookup"><span data-stu-id="08fd2-158">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="08fd2-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08fd2-159">Required.</span></span> <span data-ttu-id="08fd2-160">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="08fd2-160">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="08fd2-161">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="08fd2-161">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="08fd2-162">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-162">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="08fd2-163">clientState</span><span class="sxs-lookup"><span data-stu-id="08fd2-163">clientState</span></span> | <span data-ttu-id="08fd2-164">string</span><span class="sxs-lookup"><span data-stu-id="08fd2-164">string</span></span> | <span data-ttu-id="08fd2-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="08fd2-165">Optional.</span></span> <span data-ttu-id="08fd2-166">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="08fd2-166">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="08fd2-167">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="08fd2-167">The maximum length is 128 characters.</span></span> <span data-ttu-id="08fd2-168">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="08fd2-168">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="08fd2-169">id</span><span class="sxs-lookup"><span data-stu-id="08fd2-169">id</span></span> | <span data-ttu-id="08fd2-170">string</span><span class="sxs-lookup"><span data-stu-id="08fd2-170">string</span></span> | <span data-ttu-id="08fd2-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="08fd2-173">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="08fd2-173">applicationId</span></span> | <span data-ttu-id="08fd2-174">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08fd2-174">string</span></span> | <span data-ttu-id="08fd2-175">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-175">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="08fd2-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-176">Read-only.</span></span> |
| <span data-ttu-id="08fd2-177">creatorId</span><span class="sxs-lookup"><span data-stu-id="08fd2-177">creatorId</span></span> | <span data-ttu-id="08fd2-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08fd2-178">string</span></span> | <span data-ttu-id="08fd2-179">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-179">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="08fd2-180">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="08fd2-180">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="08fd2-181">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08fd2-181">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="08fd2-182">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-182">Read-only.</span></span> |
| <span data-ttu-id="08fd2-183">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="08fd2-183">latestSupportedTlsVersion</span></span> | <span data-ttu-id="08fd2-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08fd2-184">String</span></span> | <span data-ttu-id="08fd2-185">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="08fd2-185">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="08fd2-186">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="08fd2-186">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="08fd2-187">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="08fd2-187">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="08fd2-188">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="08fd2-188">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="08fd2-189">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="08fd2-189">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="08fd2-190">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="08fd2-190">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="08fd2-191">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="08fd2-191">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="08fd2-192">Resource</span><span class="sxs-lookup"><span data-stu-id="08fd2-192">Resource</span></span>            | <span data-ttu-id="08fd2-193">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="08fd2-193">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="08fd2-194">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="08fd2-194">User, group, other directory resources</span></span>   | <span data-ttu-id="08fd2-195">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-195">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-196">Correio</span><span class="sxs-lookup"><span data-stu-id="08fd2-196">Mail</span></span>                | <span data-ttu-id="08fd2-197">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-197">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-198">Calendário</span><span class="sxs-lookup"><span data-stu-id="08fd2-198">Calendar</span></span>            | <span data-ttu-id="08fd2-199">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-199">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-200">Contatos</span><span class="sxs-lookup"><span data-stu-id="08fd2-200">Contacts</span></span>            | <span data-ttu-id="08fd2-201">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-201">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-202">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="08fd2-202">Group conversations</span></span> | <span data-ttu-id="08fd2-203">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-203">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-204">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="08fd2-204">Drive root items</span></span>    | <span data-ttu-id="08fd2-205">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-205">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-206">Lista do SharePoint</span><span class="sxs-lookup"><span data-stu-id="08fd2-206">SharePoint list</span></span>     | <span data-ttu-id="08fd2-207">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="08fd2-207">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="08fd2-208">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="08fd2-208">Security alerts</span></span>     | <span data-ttu-id="08fd2-209">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="08fd2-209">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="08fd2-210">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="08fd2-210">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="08fd2-211">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="08fd2-211">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="08fd2-212">Relações</span><span class="sxs-lookup"><span data-stu-id="08fd2-212">Relationships</span></span>

<span data-ttu-id="08fd2-213">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08fd2-213">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08fd2-214">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08fd2-214">JSON representation</span></span>

<span data-ttu-id="08fd2-215">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08fd2-215">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "latestSupportedTlsVersion": "string"
}
```

[contato]: ./contact.md
[contact]: ./contact.md
[conversa]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

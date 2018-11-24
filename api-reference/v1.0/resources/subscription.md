# <a name="subscription-resource-type"></a><span data-ttu-id="7a5a3-101">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="7a5a3-101">subscription resource type</span></span>

<span data-ttu-id="7a5a3-102">Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-102">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="7a5a3-103">Atualmente, as assinaturas são habilitadas para os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="7a5a3-103">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="7a5a3-104">Email, eventos e contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-104">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="7a5a3-105">Conversas de Grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="7a5a3-106">Itens raiz da unidade do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-106">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="7a5a3-107">Usuários e grupos do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-107">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="7a5a3-108">Alertas do API de segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-108">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a5a3-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a5a3-109">JSON representation</span></span>

<span data-ttu-id="7a5a3-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-110">Here is a JSON representation of the resource.</span></span>

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
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="7a5a3-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a5a3-111">Properties</span></span>

| <span data-ttu-id="7a5a3-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a5a3-112">Property</span></span> | <span data-ttu-id="7a5a3-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a5a3-113">Type</span></span> | <span data-ttu-id="7a5a3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a5a3-114">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="7a5a3-115">changeType</span><span class="sxs-lookup"><span data-stu-id="7a5a3-115">changeType</span></span> | <span data-ttu-id="7a5a3-116">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-116">string</span></span> | <span data-ttu-id="7a5a3-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-117">Required.</span></span> <span data-ttu-id="7a5a3-118">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-118">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="7a5a3-119">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-119">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="7a5a3-120">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-120">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="7a5a3-121">Observação: Notificações de item de raiz de unidade suportam somente a `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-121">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="7a5a3-122">Suportam a notificações de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-122">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="7a5a3-123">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="7a5a3-123">notificationUrl</span></span> | <span data-ttu-id="7a5a3-124">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-124">string</span></span> | <span data-ttu-id="7a5a3-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-125">Required.</span></span> <span data-ttu-id="7a5a3-126">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-126">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="7a5a3-127">Essa URL deve tornar a usar o HTTPS protocolo.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-127">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="7a5a3-128">recurso</span><span class="sxs-lookup"><span data-stu-id="7a5a3-128">resource</span></span> | <span data-ttu-id="7a5a3-129">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-129">string</span></span> | <span data-ttu-id="7a5a3-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-130">Required.</span></span> <span data-ttu-id="7a5a3-131">Especifica o recurso que será monitorado para que as alterações.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-131">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="7a5a3-132">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="7a5a3-132">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="7a5a3-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7a5a3-133">expirationDateTime</span></span> | [<span data-ttu-id="7a5a3-134">dateTime</span><span class="sxs-lookup"><span data-stu-id="7a5a3-134">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="7a5a3-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-135">Required.</span></span> <span data-ttu-id="7a5a3-136">Especifica a data e a hora em que a assinatura de webhook expira.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-136">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="7a5a3-137">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-137">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="7a5a3-138">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-138">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="7a5a3-139">clientState</span><span class="sxs-lookup"><span data-stu-id="7a5a3-139">clientState</span></span> | <span data-ttu-id="7a5a3-140">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-140">string</span></span> | <span data-ttu-id="7a5a3-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-141">Optional.</span></span> <span data-ttu-id="7a5a3-142">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-142">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="7a5a3-143">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-143">The maximum length is 128 characters.</span></span> <span data-ttu-id="7a5a3-144">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-144">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="7a5a3-145">id</span><span class="sxs-lookup"><span data-stu-id="7a5a3-145">id</span></span> | <span data-ttu-id="7a5a3-146">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-146">string</span></span> | <span data-ttu-id="7a5a3-p108">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="7a5a3-149">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="7a5a3-149">applicationId</span></span> | <span data-ttu-id="7a5a3-150">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-150">string</span></span> | <span data-ttu-id="7a5a3-151">Identificador do aplicativo usado para criar a inscrição.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-151">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="7a5a3-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-152">Read-only.</span></span> |
| <span data-ttu-id="7a5a3-153">creatorId</span><span class="sxs-lookup"><span data-stu-id="7a5a3-153">creatorId</span></span> | <span data-ttu-id="7a5a3-154">string</span><span class="sxs-lookup"><span data-stu-id="7a5a3-154">string</span></span> | <span data-ttu-id="7a5a3-155">Identificador do usuário ou da entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-155">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="7a5a3-156">Se o aplicativo usado delegadas permissões para criar a assinatura, esse campo contém a id do usuário entrou no de que aplicativo chamado em nome.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-156">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="7a5a3-157">Se o aplicativo usado permissões de aplicativo, esse campo contém a id da entidade de serviço correspondente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-157">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="7a5a3-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-158">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="7a5a3-159">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="7a5a3-159">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="7a5a3-160">Recurso</span><span class="sxs-lookup"><span data-stu-id="7a5a3-160">Resource</span></span>            | <span data-ttu-id="7a5a3-161">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="7a5a3-161">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="7a5a3-162">Email</span><span class="sxs-lookup"><span data-stu-id="7a5a3-162">Mail</span></span>                | <span data-ttu-id="7a5a3-163">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="7a5a3-163">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7a5a3-164">Calendário</span><span class="sxs-lookup"><span data-stu-id="7a5a3-164">Calendar</span></span>            | <span data-ttu-id="7a5a3-165">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="7a5a3-165">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7a5a3-166">Contatos</span><span class="sxs-lookup"><span data-stu-id="7a5a3-166">Contacts</span></span>            | <span data-ttu-id="7a5a3-167">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="7a5a3-167">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7a5a3-168">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="7a5a3-168">Group conversations</span></span> | <span data-ttu-id="7a5a3-169">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="7a5a3-169">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7a5a3-170">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="7a5a3-170">Drive root items</span></span>    | <span data-ttu-id="7a5a3-171">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="7a5a3-171">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7a5a3-172">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="7a5a3-172">Security alerts</span></span>     | <span data-ttu-id="7a5a3-173">43200 minutos (em 30 dias)</span><span class="sxs-lookup"><span data-stu-id="7a5a3-173">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="7a5a3-174">**Observação:** Aplicativos existentes e novos não deve exceder o valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-174">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="7a5a3-175">No futuro, quaisquer solicitações para criar ou renovar uma assinatura além o valor máximo falhará.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-175">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="7a5a3-176">Relações</span><span class="sxs-lookup"><span data-stu-id="7a5a3-176">Relationships</span></span>

<span data-ttu-id="7a5a3-177">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a5a3-177">None</span></span>

## <a name="methods"></a><span data-ttu-id="7a5a3-178">Métodos</span><span class="sxs-lookup"><span data-stu-id="7a5a3-178">Methods</span></span>

| <span data-ttu-id="7a5a3-179">Método</span><span class="sxs-lookup"><span data-stu-id="7a5a3-179">Method</span></span> | <span data-ttu-id="7a5a3-180">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7a5a3-180">Return Type</span></span> | <span data-ttu-id="7a5a3-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a5a3-181">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="7a5a3-182">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="7a5a3-182">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="7a5a3-183">subscription</span><span class="sxs-lookup"><span data-stu-id="7a5a3-183">subscription</span></span>](subscription.md) | <span data-ttu-id="7a5a3-184">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-184">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="7a5a3-185">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="7a5a3-185">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="7a5a3-186">subscription</span><span class="sxs-lookup"><span data-stu-id="7a5a3-186">subscription</span></span>](subscription.md) | <span data-ttu-id="7a5a3-187">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-187">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="7a5a3-188">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="7a5a3-188">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="7a5a3-189">subscription</span><span class="sxs-lookup"><span data-stu-id="7a5a3-189">subscription</span></span>](subscription.md) | <span data-ttu-id="7a5a3-190">Lista inscrições ativas.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-190">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="7a5a3-191">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="7a5a3-191">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="7a5a3-192">subscription</span><span class="sxs-lookup"><span data-stu-id="7a5a3-192">subscription</span></span>](subscription.md) | <span data-ttu-id="7a5a3-193">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-193">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="7a5a3-194">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="7a5a3-194">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="7a5a3-195">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7a5a3-195">None</span></span> |<span data-ttu-id="7a5a3-196">Exclui um objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="7a5a3-196">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="subscription-resource-type"></a><span data-ttu-id="5e470-101">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-101">Subscription resource type</span></span>

<span data-ttu-id="5e470-102">Uma assinatura permite que um aplicativo cliente receba notificações sobre as alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5e470-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="5e470-103">Atualmente, as assinaturas são habilitadas para os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="5e470-103">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="5e470-104">Email, eventos e contatos do Outlook</span><span class="sxs-lookup"><span data-stu-id="5e470-104">Mail, events, and contacts from Outlook</span></span>
- <span data-ttu-id="5e470-105">Conversas de Grupos do Office</span><span class="sxs-lookup"><span data-stu-id="5e470-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="5e470-106">Itens raiz de unidade no OneDrive</span><span class="sxs-lookup"><span data-stu-id="5e470-106">Drive root items from OneDrive</span></span>
- <span data-ttu-id="5e470-107">Usuários e grupos do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5e470-107">Users and Groups from Azure Active Directory</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e470-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e470-108">JSON representation</span></span>

<span data-ttu-id="5e470-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e470-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5e470-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e470-110">Properties</span></span>

| <span data-ttu-id="5e470-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e470-111">Property</span></span> | <span data-ttu-id="5e470-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e470-112">Type</span></span> | <span data-ttu-id="5e470-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e470-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5e470-114">changeType</span><span class="sxs-lookup"><span data-stu-id="5e470-114">changeType</span></span> | <span data-ttu-id="5e470-115">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-115">string</span></span> | <span data-ttu-id="5e470-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e470-116">Required.</span></span> <span data-ttu-id="5e470-117">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="5e470-117">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="5e470-118">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="5e470-118">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="5e470-119">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="5e470-119">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="5e470-120">Nota: Notificações de item de raiz de unidade suportam somente a `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="5e470-120">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="5e470-121">Suporte a notificações de usuários e grupos `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="5e470-121">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="5e470-122">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="5e470-122">notificationUrl</span></span> | <span data-ttu-id="5e470-123">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-123">string</span></span> | <span data-ttu-id="5e470-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e470-124">Required.</span></span> <span data-ttu-id="5e470-125">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="5e470-125">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="5e470-126">Essa URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5e470-126">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="5e470-127">recurso</span><span class="sxs-lookup"><span data-stu-id="5e470-127">resource</span></span> | <span data-ttu-id="5e470-128">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-128">string</span></span> | <span data-ttu-id="5e470-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e470-129">Required.</span></span> <span data-ttu-id="5e470-130">Especifica o recurso cujas alterações serão monitoradas.</span><span class="sxs-lookup"><span data-stu-id="5e470-130">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span> <span data-ttu-id="5e470-131">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="5e470-131">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="5e470-132">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5e470-132">expirationDateTime</span></span> | [<span data-ttu-id="5e470-133">dateTime</span><span class="sxs-lookup"><span data-stu-id="5e470-133">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="5e470-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e470-134">Required.</span></span> <span data-ttu-id="5e470-135">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="5e470-135">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="5e470-136">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="5e470-136">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="5e470-137">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="5e470-137">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="5e470-138">clientState</span><span class="sxs-lookup"><span data-stu-id="5e470-138">clientState</span></span> | <span data-ttu-id="5e470-139">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-139">string</span></span> | <span data-ttu-id="5e470-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5e470-140">Optional.</span></span> <span data-ttu-id="5e470-141">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="5e470-141">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="5e470-142">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="5e470-142">The maximum length is 128 characters.</span></span> <span data-ttu-id="5e470-143">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="5e470-143">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="5e470-144">id</span><span class="sxs-lookup"><span data-stu-id="5e470-144">id</span></span> | <span data-ttu-id="5e470-145">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-145">string</span></span> | <span data-ttu-id="5e470-p108">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e470-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="5e470-148">applicationId</span><span class="sxs-lookup"><span data-stu-id="5e470-148">applicationId</span></span> | <span data-ttu-id="5e470-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-149">string</span></span> | <span data-ttu-id="5e470-150">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="5e470-150">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="5e470-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e470-151">Read-only.</span></span> |
| <span data-ttu-id="5e470-152">creatorId</span><span class="sxs-lookup"><span data-stu-id="5e470-152">creatorId</span></span> | <span data-ttu-id="5e470-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e470-153">string</span></span> | <span data-ttu-id="5e470-154">Identificador do usuário ou da entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="5e470-154">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="5e470-155">Se o aplicativo usou permissões delegadas para criar a assinatura, esse campo contém o ID do usuário conectado em nome do qual o aplicativo foi chamado.</span><span class="sxs-lookup"><span data-stu-id="5e470-155">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="5e470-156">Se o aplicativo usou as permissões do aplicativo, esse campo contém o id da entidade de serviço correspondente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5e470-156">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="5e470-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e470-157">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="5e470-158">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="5e470-158">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="5e470-159">Recurso</span><span class="sxs-lookup"><span data-stu-id="5e470-159">Resource</span></span>            | <span data-ttu-id="5e470-160">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="5e470-160">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="5e470-161">Email</span><span class="sxs-lookup"><span data-stu-id="5e470-161">Mail</span></span>                | <span data-ttu-id="5e470-162">4230 minutos (menos de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="5e470-162">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5e470-163">Calendário</span><span class="sxs-lookup"><span data-stu-id="5e470-163">Calendar</span></span>            | <span data-ttu-id="5e470-164">4230 minutos (menos de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="5e470-164">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5e470-165">Contatos</span><span class="sxs-lookup"><span data-stu-id="5e470-165">Contacts</span></span>            | <span data-ttu-id="5e470-166">4230 minutos (menos de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="5e470-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5e470-167">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="5e470-167">Group conversations</span></span> | <span data-ttu-id="5e470-168">4230 minutos (menos de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="5e470-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5e470-169">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="5e470-169">Drive root items</span></span>    | <span data-ttu-id="5e470-170">4230 minutos (menos de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="5e470-170">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="5e470-171">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor máximo.</span><span class="sxs-lookup"><span data-stu-id="5e470-171">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="5e470-172">No futuro, quaisquer solicitações para criar ou renovar uma assinatura além do valor máximo, falhará.</span><span class="sxs-lookup"><span data-stu-id="5e470-172">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="5e470-173">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="5e470-173">Relationships</span></span>

<span data-ttu-id="5e470-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e470-174">None</span></span>

## <a name="methods"></a><span data-ttu-id="5e470-175">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e470-175">Methods</span></span>

| <span data-ttu-id="5e470-176">Método</span><span class="sxs-lookup"><span data-stu-id="5e470-176">Method</span></span> | <span data-ttu-id="5e470-177">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e470-177">Return Type</span></span> | <span data-ttu-id="5e470-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e470-178">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="5e470-179">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-179">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="5e470-180">assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-180">subscription</span></span>](subscription.md) | <span data-ttu-id="5e470-181">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="5e470-181">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="5e470-182">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-182">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="5e470-183">assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-183">subscription</span></span>](subscription.md) | <span data-ttu-id="5e470-184">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="5e470-184">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="5e470-185">Assinaturas de lista</span><span class="sxs-lookup"><span data-stu-id="5e470-185">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="5e470-186">assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-186">subscription</span></span>](subscription.md) | <span data-ttu-id="5e470-187">Lista as assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="5e470-187">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="5e470-188">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-188">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="5e470-189">assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-189">subscription</span></span>](subscription.md) | <span data-ttu-id="5e470-190">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="5e470-190">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="5e470-191">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="5e470-191">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="5e470-192">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5e470-192">None</span></span> |<span data-ttu-id="5e470-193">Exclui um objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="5e470-193">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

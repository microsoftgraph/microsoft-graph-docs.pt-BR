# <a name="subscription-resource-type"></a><span data-ttu-id="29bde-101">Tipo de Recurso de Assinatura</span><span class="sxs-lookup"><span data-stu-id="29bde-101">Subscription Resource Type</span></span>
<span data-ttu-id="29bde-102">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="29bde-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph. Currently subscriptions are enabled for the following datasets:</span></span> <span data-ttu-id="29bde-103">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de dados:</span><span class="sxs-lookup"><span data-stu-id="29bde-103">Currently, subscriptions are enabled for the following datasets:</span></span>

1. <span data-ttu-id="29bde-104">Email, eventos e contatos do Outlook</span><span class="sxs-lookup"><span data-stu-id="29bde-104">Mail, events, and contacts from Outlook</span></span>
1. <span data-ttu-id="29bde-105">Conversas de Grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="29bde-105">Conversations from Office Groups.</span></span>
1. <span data-ttu-id="29bde-106">Itens raiz de unidade no OneDrive</span><span class="sxs-lookup"><span data-stu-id="29bde-106">Drive root items from OneDrive</span></span> 


## <a name="json-representation"></a><span data-ttu-id="29bde-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29bde-107">JSON representation</span></span>

<span data-ttu-id="29bde-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29bde-108">Here is a JSON representation of the resource.</span></span>

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
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a><span data-ttu-id="29bde-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29bde-109">Properties</span></span>
| <span data-ttu-id="29bde-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29bde-110">Property</span></span>     | <span data-ttu-id="29bde-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="29bde-111">Type</span></span>   |<span data-ttu-id="29bde-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="29bde-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29bde-113">changeType</span><span class="sxs-lookup"><span data-stu-id="29bde-113">changeType</span></span>|<span data-ttu-id="29bde-114">string</span><span class="sxs-lookup"><span data-stu-id="29bde-114">string</span></span>|<span data-ttu-id="29bde-115">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="29bde-115">Indicates the type of change in the subscribed resource that will raise a notification. The supported values are: , , . Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="29bde-116">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="29bde-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="29bde-117">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="29bde-117">Multiple values can be combined using a comma-separated list.</span></span>|
|<span data-ttu-id="29bde-118">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="29bde-118">notificationUrl</span></span>|<span data-ttu-id="29bde-119">string</span><span class="sxs-lookup"><span data-stu-id="29bde-119">string</span></span>|<span data-ttu-id="29bde-p103">A URL do ponto de extremidade que receberá as notificações. Esta URL tem que usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="29bde-p103">The URL of the endpoint that will receive the notifications. This URL has to make use of the HTTPS protocol.</span></span>|
|<span data-ttu-id="29bde-122">recurso</span><span class="sxs-lookup"><span data-stu-id="29bde-122">resource</span></span>|<span data-ttu-id="29bde-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29bde-123">string</span></span>|<span data-ttu-id="29bde-p104">Especifica o recurso que será monitorado para detectar alterações. Não inclua a URL base ("https://graph.microsoft.com/v1.0/").</span><span class="sxs-lookup"><span data-stu-id="29bde-p104">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span>|
|<span data-ttu-id="29bde-126">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="29bde-126">expirationDateTime</span></span>|[<span data-ttu-id="29bde-127">dateTime</span><span class="sxs-lookup"><span data-stu-id="29bde-127">dateTime</span></span>](http://tools.ietf.org/html/rfc3339)|<span data-ttu-id="29bde-128">Especifica a data e a hora em que a assinatura de webhook expira.</span><span class="sxs-lookup"><span data-stu-id="29bde-128">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="29bde-129">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="29bde-129">Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.  See the table below for maximum values.</span></span>  <span data-ttu-id="29bde-130">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="29bde-130">See the table below for maximum supported subscription length of time.</span></span> |
|<span data-ttu-id="29bde-131">clientState</span><span class="sxs-lookup"><span data-stu-id="29bde-131">clientState</span></span>|<span data-ttu-id="29bde-132">string</span><span class="sxs-lookup"><span data-stu-id="29bde-132">string</span></span>|<span data-ttu-id="29bde-133">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="29bde-133">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="29bde-134">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="29bde-134">The maximum length is 255 characters.</span></span> <span data-ttu-id="29bde-135">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="29bde-135">Specifies the value of the  property sent by the service in each notification. The maximum length is 128 characters. The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span>|
|<span data-ttu-id="29bde-136">id</span><span class="sxs-lookup"><span data-stu-id="29bde-136">id</span></span>|<span data-ttu-id="29bde-137">string</span><span class="sxs-lookup"><span data-stu-id="29bde-137">string</span></span>|<span data-ttu-id="29bde-p107">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29bde-p107">Unique identifier for the subscription. Read-only.</span></span>|

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="29bde-140">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="29bde-140">Maximum length of subscription per resource type</span></span>
| <span data-ttu-id="29bde-141">Recurso</span><span class="sxs-lookup"><span data-stu-id="29bde-141">Resource</span></span> | <span data-ttu-id="29bde-142">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="29bde-142">Maximum Expiration Time</span></span> |
|:---------------------|:--------------------|
|<span data-ttu-id="29bde-143">Email</span><span class="sxs-lookup"><span data-stu-id="29bde-143">Mail</span></span>| <span data-ttu-id="29bde-144">4230 minutos.</span><span class="sxs-lookup"><span data-stu-id="29bde-144">4230 minutes.</span></span>|
|<span data-ttu-id="29bde-145">Calendário</span><span class="sxs-lookup"><span data-stu-id="29bde-145">Calendar</span></span>| <span data-ttu-id="29bde-146">4230 minutos.</span><span class="sxs-lookup"><span data-stu-id="29bde-146">4230 minutes.</span></span>|
|<span data-ttu-id="29bde-147">Contatos</span><span class="sxs-lookup"><span data-stu-id="29bde-147">Contacts</span></span>| <span data-ttu-id="29bde-148">4230 minutos.</span><span class="sxs-lookup"><span data-stu-id="29bde-148">4230 minutes.</span></span>|
|<span data-ttu-id="29bde-149">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="29bde-149">Group conversations</span></span>| <span data-ttu-id="29bde-150">4230 minutos.</span><span class="sxs-lookup"><span data-stu-id="29bde-150">4230 minutes.</span></span>|
|<span data-ttu-id="29bde-151">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="29bde-151">Drive root items</span></span>| <span data-ttu-id="29bde-152">43.200 minutos.</span><span class="sxs-lookup"><span data-stu-id="29bde-152">43200 minutes.</span></span> <span data-ttu-id="29bde-153">Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor máximo.</span><span class="sxs-lookup"><span data-stu-id="29bde-153">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="29bde-154">Valores maiores não serão permitidos nos próximos lançamentos.</span><span class="sxs-lookup"><span data-stu-id="29bde-154">Higher values won't be permitted in upcoming releases.</span></span> |

## <a name="relationships"></a><span data-ttu-id="29bde-155">Relações</span><span class="sxs-lookup"><span data-stu-id="29bde-155">Relationships</span></span>
<span data-ttu-id="29bde-156">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="29bde-156">None</span></span>


## <a name="methods"></a><span data-ttu-id="29bde-157">Métodos</span><span class="sxs-lookup"><span data-stu-id="29bde-157">Methods</span></span>

| <span data-ttu-id="29bde-158">Método</span><span class="sxs-lookup"><span data-stu-id="29bde-158">Method</span></span>           | <span data-ttu-id="29bde-159">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29bde-159">Return Type</span></span>    |<span data-ttu-id="29bde-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="29bde-160">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29bde-161">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="29bde-161">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="29bde-162">subscription</span><span class="sxs-lookup"><span data-stu-id="29bde-162">subscription</span></span>](subscription.md) |<span data-ttu-id="29bde-163">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="29bde-163">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span>|
|[<span data-ttu-id="29bde-164">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="29bde-164">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="29bde-165">subscription</span><span class="sxs-lookup"><span data-stu-id="29bde-165">subscription</span></span>](subscription.md) |<span data-ttu-id="29bde-166">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="29bde-166">Renews a subscription by updating its expiration time.</span></span>|
|[<span data-ttu-id="29bde-167">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="29bde-167">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="29bde-168">subscription</span><span class="sxs-lookup"><span data-stu-id="29bde-168">subscription</span></span>](subscription.md) |<span data-ttu-id="29bde-169">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="29bde-169">Reads properties and relationships of subscription object.</span></span>|
|[<span data-ttu-id="29bde-170">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="29bde-170">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="29bde-171">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="29bde-171">None</span></span> |<span data-ttu-id="29bde-172">Exclui um objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="29bde-172">Deletes a subscription object.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

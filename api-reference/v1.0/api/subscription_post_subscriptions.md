# <a name="create-subscription"></a><span data-ttu-id="d0dac-101">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="d0dac-101">Create subscription</span></span>

<span data-ttu-id="d0dac-102">Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="d0dac-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0dac-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0dac-103">Permissions</span></span>
<span data-ttu-id="d0dac-p101">Criar uma assinatura exige escopo de leitura para o recurso. Por exemplo, para obter mensagens de notificações, seu aplicativo precisa da permissão `Mail.Read`. A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0dac-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d0dac-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="d0dac-108">Resource type / Item</span></span>        | <span data-ttu-id="d0dac-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="d0dac-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="d0dac-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="d0dac-110">Contacts</span></span>                    | <span data-ttu-id="d0dac-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d0dac-111">Contacts.Read</span></span>       |
| <span data-ttu-id="d0dac-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="d0dac-112">Conversations</span></span>               | <span data-ttu-id="d0dac-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0dac-113">Group.Read.All</span></span>      |
| <span data-ttu-id="d0dac-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="d0dac-114">Events</span></span>                      | <span data-ttu-id="d0dac-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d0dac-115">Calendars.Read</span></span>      |
| <span data-ttu-id="d0dac-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="d0dac-116">Messages</span></span>                    | <span data-ttu-id="d0dac-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d0dac-117">Mail.Read</span></span>           |
| <span data-ttu-id="d0dac-118">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="d0dac-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d0dac-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0dac-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d0dac-120">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="d0dac-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="d0dac-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0dac-121">Files.ReadWrite.All</span></span> |

 <span data-ttu-id="d0dac-p102">***Observação:*** O ponto de extremidade /v1.0 dá permissões do aplicativo para a maioria dos recursos. Não há suporte para conversas em grupo e itens da unidade raiz do OneDrive com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0dac-p102">One of the following scopes, depending on the target resource, are required to execute this API: Mail.Read, Calendars.Read, Contacts.Read, Group.Read.All, Files.ReadWrite or Files.ReadWrite.All. ***Note:*** The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0dac-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0dac-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a><span data-ttu-id="d0dac-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0dac-125">Request headers</span></span>
| <span data-ttu-id="d0dac-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d0dac-126">Name</span></span>       | <span data-ttu-id="d0dac-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0dac-127">Type</span></span> | <span data-ttu-id="d0dac-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0dac-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0dac-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0dac-129">Authorization</span></span>  | <span data-ttu-id="d0dac-130">string</span><span class="sxs-lookup"><span data-stu-id="d0dac-130">string</span></span>  | <span data-ttu-id="d0dac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0dac-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d0dac-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0dac-133">Response</span></span>

<span data-ttu-id="d0dac-134">Se bem-sucedido, este método retorna o código de resposta `201, Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0dac-134">If successful, this method returns `201, Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0dac-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0dac-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0dac-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0dac-136">Request</span></span>
<span data-ttu-id="d0dac-137">Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="d0dac-137">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "subscription-identifier"
}
```
<span data-ttu-id="d0dac-p104">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md). O campo *clientState* é opcional.</span><span class="sxs-lookup"><span data-stu-id="d0dac-p104">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object. The *clientState* field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="d0dac-140">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="d0dac-140">Resources examples</span></span>
<span data-ttu-id="d0dac-141">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="d0dac-141">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="d0dac-142">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="d0dac-142">Resource type</span></span> | <span data-ttu-id="d0dac-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0dac-143">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="d0dac-144">Email</span><span class="sxs-lookup"><span data-stu-id="d0dac-144">Mail</span></span>|<span data-ttu-id="d0dac-145">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="d0dac-145">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="d0dac-146">me/messages</span><span class="sxs-lookup"><span data-stu-id="d0dac-146">me/messages</span></span>|
|<span data-ttu-id="d0dac-147">Contatos</span><span class="sxs-lookup"><span data-stu-id="d0dac-147">Contacts</span></span>|<span data-ttu-id="d0dac-148">me/contacts</span><span class="sxs-lookup"><span data-stu-id="d0dac-148">me/contacts</span></span>|
|<span data-ttu-id="d0dac-149">Calendários</span><span class="sxs-lookup"><span data-stu-id="d0dac-149">Calendars</span></span>|<span data-ttu-id="d0dac-150">me/events</span><span class="sxs-lookup"><span data-stu-id="d0dac-150">me/events</span></span>|
|<span data-ttu-id="d0dac-151">Conversas</span><span class="sxs-lookup"><span data-stu-id="d0dac-151">Conversations</span></span>|<span data-ttu-id="d0dac-152">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="d0dac-152">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="d0dac-153">Unidades</span><span class="sxs-lookup"><span data-stu-id="d0dac-153">Drives</span></span>|<span data-ttu-id="d0dac-154">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="d0dac-154">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="d0dac-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0dac-155">Response</span></span>
<span data-ttu-id="d0dac-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0dac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a><span data-ttu-id="d0dac-159">Validação de assinaturas</span><span class="sxs-lookup"><span data-stu-id="d0dac-159">Subscription validation</span></span>
<span data-ttu-id="d0dac-p106">Para evitar que assinaturas incorretas direcionem notificações para URLs arbitrárias, o ponto de extremidade de notificação de assinatura deve ser capaz de responder a uma solicitação de validação. Durante o processamento de `POST` para o ponto de extremidade `/subscriptions`, o Microsoft Graph enviará uma solicitação `POST` de volta ao seu `notificationUrl`, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="d0dac-p106">In order to to avoid mistaken subscriptions directing notifications to arbitrary URLs, the subscription notification endpoint must be capable of responding to a validation request. During processing of the `POST` to the `/subscriptions` endpoint, the Microsoft Graph will send a `POST` request back to your `notificationUrl` in the following form:</span></span> 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
<span data-ttu-id="d0dac-162">O ponto de extremidade de notificação deve enviar uma resposta 200 com o valor de `<token>` como o corpo e um tipo de conteúdo de `text/plain`, conforme mostrado abaixo, dentro de 10 segundos. Caso contrário, a solicitação de criação será descartada.</span><span class="sxs-lookup"><span data-stu-id="d0dac-162">The notification endpoint must send a 200 response with the value of `<token>` as its body and a content type of `text/plain`, as shown below, within 10 seconds otherwise the creation request will be discarded.</span></span>
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a><span data-ttu-id="d0dac-163">Carga de notificação</span><span class="sxs-lookup"><span data-stu-id="d0dac-163">Notification payload</span></span>
<span data-ttu-id="d0dac-p107">Quando o recurso assinado mudar, a as alterações de recurso inscrito, as instalações de webhooks enviarão uma notificação para a URL de notificação com a seguinte carga.  O ponto de extremidade de notificação deve enviar uma resposta de 200 ou 204 sem um corpo de resposta dentro de 30 segundos. Caso contrário, a tentativa de notificação será repetida em intervalos exponencialmente crescentes.  Os serviços que demoram consistentemente 30 segundos ou mais podem ser limitados e recebem um conjunto de notificação mais esparso.</span><span class="sxs-lookup"><span data-stu-id="d0dac-p107">When the subscribed resource changes, the webhooks facility sends a notification to your notification URL with the following payload.  The notification endpoint must send a response of 200 or 204 with no response body within 30 seconds otherwise the notification attempt will be retried at exponentially increasing intervals.  Services that consistently take 30 seconds or more may be throttled and receive a sparser notification set.</span></span>

<span data-ttu-id="d0dac-167">Os serviços também podem retornar uma resposta 422 de uma notificação. Nesse caso, a assinatura será automaticamente excluída, e o fluxo de notificações será interrompido.</span><span class="sxs-lookup"><span data-stu-id="d0dac-167">Services may also return a 422 response from a notification, in which case the subscription will be automatically deleted and the stream of notifications will come to a halt.</span></span>

<span data-ttu-id="d0dac-168">Dependendo do recurso assinado, um campo resourceData adicional pode fornecer informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d0dac-168">Depending on the subscribed resource, an additional resourceData field may provide additional information.</span></span>

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
<span data-ttu-id="d0dac-p108">Ao receber notificações de assinaturas de Drive, resourceData será nulo, e a API [delta](item_delta.md) deverá ser chamada para determinar as alterações que ocorreram. Veja a seguir um exemplo de notificação de Drive:</span><span class="sxs-lookup"><span data-stu-id="d0dac-p108">When receiving notifications from Drive subscriptions the resourceData will be null and the [delta](item_delta.md) API should be called to determine the changes that have occured. Here is an example of a Drive notification:</span></span>
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

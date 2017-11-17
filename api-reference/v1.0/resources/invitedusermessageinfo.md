# <a name="configuring-the-invitation-message"></a><span data-ttu-id="4d268-101">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="4d268-101">Configuring the invitation message</span></span>

<span data-ttu-id="4d268-102">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="4d268-102">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="4d268-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d268-103">Properties</span></span>
| <span data-ttu-id="4d268-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d268-104">Property</span></span>     | <span data-ttu-id="4d268-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d268-105">Type</span></span>   |<span data-ttu-id="4d268-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d268-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d268-107">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="4d268-107">ccRecipients</span></span>|[<span data-ttu-id="4d268-108">Recipient</span><span class="sxs-lookup"><span data-stu-id="4d268-108">Recipient</span></span>](recipient.md)|<span data-ttu-id="4d268-p101">Outros destinatários aos quais a mensagem de convite deve ser enviada. No momento, só é possível adicionar mais um destinatário.</span><span class="sxs-lookup"><span data-stu-id="4d268-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="4d268-111">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="4d268-111">customizedMessageBody</span></span>|<span data-ttu-id="4d268-112">String</span><span class="sxs-lookup"><span data-stu-id="4d268-112">String</span></span>|<span data-ttu-id="4d268-113">Corpo da mensagem personalizada a ser enviada caso você não queira a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="4d268-113">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="4d268-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="4d268-114">messageLanguage</span></span>|<span data-ttu-id="4d268-115">String</span><span class="sxs-lookup"><span data-stu-id="4d268-115">String</span></span>|<span data-ttu-id="4d268-p102">O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificada, essa propriedade será ignorada, e a mensagem será enviada usando-se customizedMessageBody. O formato do idioma deve estar no ISO 639. O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="4d268-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d268-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d268-120">JSON representation</span></span>
<span data-ttu-id="4d268-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4d268-121">Here is a JSON representation of the resource</span></span>

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

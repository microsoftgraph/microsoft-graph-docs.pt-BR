# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="ae63c-101">Tipo de recurso automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="ae63c-101">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="ae63c-p101">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails.</span><span class="sxs-lookup"><span data-stu-id="ae63c-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="ae63c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae63c-104">Properties</span></span>
| <span data-ttu-id="ae63c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae63c-105">Property</span></span>     | <span data-ttu-id="ae63c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae63c-106">Type</span></span>   |<span data-ttu-id="ae63c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae63c-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae63c-108">externalAudience</span><span class="sxs-lookup"><span data-stu-id="ae63c-108">externalAudience</span></span>|<span data-ttu-id="ae63c-109">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="ae63c-109">ExternalAudienceScope</span></span>| <span data-ttu-id="ae63c-110">O conjunto de audiência externa à organização do usuário conectado que receberá **ExternalReplyMessage**, se o **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-110">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or . Possible values are: , , `Scheduled`.</span></span> <span data-ttu-id="ae63c-111">Os valores possíveis são: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-111">The possible values are:</span></span>|
|<span data-ttu-id="ae63c-112">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="ae63c-112">externalReplyMessage</span></span>|<span data-ttu-id="ae63c-113">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae63c-113">string</span></span>|<span data-ttu-id="ae63c-114">A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-114">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="ae63c-115">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="ae63c-115">internalReplyMessage</span></span>|<span data-ttu-id="ae63c-116">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae63c-116">string</span></span>|<span data-ttu-id="ae63c-117">A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-117">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="ae63c-118">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="ae63c-118">scheduledEndDateTime</span></span>|[<span data-ttu-id="ae63c-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ae63c-119">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ae63c-120">A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-120">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="ae63c-121">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ae63c-121">scheduledStartDateTime</span></span>|[<span data-ttu-id="ae63c-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ae63c-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ae63c-123">A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-123">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="ae63c-124">status</span><span class="sxs-lookup"><span data-stu-id="ae63c-124">status</span></span>|<span data-ttu-id="ae63c-125">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="ae63c-125">AutomaticRepliesStatus</span></span>|<span data-ttu-id="ae63c-126">Status configurado para respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="ae63c-126">Configurations status for automatic replies. Possible values are: , , .</span></span> <span data-ttu-id="ae63c-127">Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ae63c-127">The possible values are:</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae63c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae63c-128">JSON representation</span></span>

<span data-ttu-id="ae63c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae63c-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

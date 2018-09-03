# <a name="mailtips-resource-type"></a><span data-ttu-id="145cd-101">tipo de recurso mailTips</span><span class="sxs-lookup"><span data-stu-id="145cd-101">mailTips resource type</span></span>

<span data-ttu-id="145cd-102">Mensagens informativas sobre um destinatário, que são exibidas para os usuários ao redigir uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="145cd-102">Informative messages displayed to users while they are composing a message.</span></span> <span data-ttu-id="145cd-103">Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário da mensagem.</span><span class="sxs-lookup"><span data-stu-id="145cd-103">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="145cd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="145cd-104">Properties</span></span>
| <span data-ttu-id="145cd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="145cd-105">Property</span></span>     | <span data-ttu-id="145cd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="145cd-106">Type</span></span>   |<span data-ttu-id="145cd-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="145cd-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="145cd-108">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="145cd-108">AutomaticReplies</span></span> | [<span data-ttu-id="145cd-109">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="145cd-109">AutomaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="145cd-110">Dicas de e-mail sobre respostas automáticas, caso tenham sido configuradas pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="145cd-110">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="145cd-111">customMailTip</span><span class="sxs-lookup"><span data-stu-id="145cd-111">CustomMailTip</span></span> | <span data-ttu-id="145cd-112">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="145cd-112">String</span></span> | <span data-ttu-id="145cd-113">Uma dica de e-mail personalizada que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="145cd-113">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="145cd-114">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="145cd-114">DeliveryRestricted</span></span>| <span data-ttu-id="145cd-115">Booleano</span><span class="sxs-lookup"><span data-stu-id="145cd-115">Boolean</span></span> | <span data-ttu-id="145cd-116">Caso a caixa de correio do destinatário está restrita ou não, por exemplo, aceitando mensagens apenas de uma lista predefinida de remetentes, rejeitando mensagens de uma lista predefinida de remetentes ou aceitando mensagens apenas de remetentes autenticados.</span><span class="sxs-lookup"><span data-stu-id="145cd-116">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="145cd-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="145cd-117">emailAddress</span></span> | [<span data-ttu-id="145cd-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="145cd-118">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="145cd-119">O endereço de e-mail do destinatário que receberá as dicas de e-mail.</span><span class="sxs-lookup"><span data-stu-id="145cd-119">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="145cd-120">error</span><span class="sxs-lookup"><span data-stu-id="145cd-120">error</span></span> | [<span data-ttu-id="145cd-121">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="145cd-121">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="145cd-122">Erros que ocorrem durante a ação [GetMailTips](../api/user_getmailtips.md).</span><span class="sxs-lookup"><span data-stu-id="145cd-122">Errors that occur during the [GetMailTips](../api/user_getmailtips.md) action.</span></span> |
| <span data-ttu-id="145cd-123">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="145cd-123">ExternalMemberCount</span></span> | <span data-ttu-id="145cd-124">Int32</span><span class="sxs-lookup"><span data-stu-id="145cd-124">Int32</span></span> | <span data-ttu-id="145cd-125">O número de membros externos, se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="145cd-125">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="145cd-126">isModerated</span><span class="sxs-lookup"><span data-stu-id="145cd-126">IsModerated</span></span> |<span data-ttu-id="145cd-127">Booleano</span><span class="sxs-lookup"><span data-stu-id="145cd-127">Boolean</span></span>  | <span data-ttu-id="145cd-128">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="145cd-128">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="145cd-129">Por exemplo, se o destinatário for uma grande lista de distribuição e um moderador tiver sido configurado para aprovar mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário exigir a aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="145cd-129">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="145cd-130">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="145cd-130">MailboxFull</span></span> | <span data-ttu-id="145cd-131">Booleano</span><span class="sxs-lookup"><span data-stu-id="145cd-131">Boolean</span></span> | <span data-ttu-id="145cd-132">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="145cd-132">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="145cd-133">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="145cd-133">MaxMessageSize</span></span> | <span data-ttu-id="145cd-134">Int32</span><span class="sxs-lookup"><span data-stu-id="145cd-134">Int32</span></span> | <span data-ttu-id="145cd-135">O tamanho máximo da mensagem que foi configurado para a organização ou caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="145cd-135">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="145cd-136">recipientScope</span><span class="sxs-lookup"><span data-stu-id="145cd-136">RecipientScope</span></span> | <span data-ttu-id="145cd-137">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="145cd-137">String</span></span> | <span data-ttu-id="145cd-138">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="145cd-138">The scope of the recipient, such as internal, external, partner.</span></span> <span data-ttu-id="145cd-139">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="145cd-139">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="145cd-140">Por exemplo, um administrador pode definir outra organização como "parceira".</span><span class="sxs-lookup"><span data-stu-id="145cd-140">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="145cd-141">O escopo é útil se um administrador quiser que determinadas dicas de e-mail estejam acessíveis a determinados escopos.</span><span class="sxs-lookup"><span data-stu-id="145cd-141">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="145cd-142">Também é útil para os remetentes informá-los de que a mensagem pode sair da organização, ajudando-os a tomar as decisões corretas sobre texto, tom e conteúdo.</span><span class="sxs-lookup"><span data-stu-id="145cd-142">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="145cd-143">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="145cd-143">RecipientSuggestions</span></span> | <span data-ttu-id="145cd-144">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="145cd-144">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="145cd-145">Destinatários sugeridos com base em contextos anteriores em que aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="145cd-145">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="145cd-146">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="145cd-146">TotalMemberCount</span></span> | <span data-ttu-id="145cd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="145cd-147">Int32</span></span> | <span data-ttu-id="145cd-148">O número de membros, se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="145cd-148">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="145cd-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="145cd-149">JSON representation</span></span>

<span data-ttu-id="145cd-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="145cd-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
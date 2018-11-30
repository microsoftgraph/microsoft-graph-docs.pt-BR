---
title: tipo de recurso de dicas de email
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem. Por exemplo, uma mensagem de ausência temporária '
ms.openlocfilehash: 6c5d64248aa940b9449a93caad952bc7b4d13ca6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004451"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="4de1c-104">tipo de recurso de dicas de email</span><span class="sxs-lookup"><span data-stu-id="4de1c-104">mailTips resource type</span></span>

<span data-ttu-id="4de1c-105">Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="4de1c-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="4de1c-106">Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.</span><span class="sxs-lookup"><span data-stu-id="4de1c-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="4de1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4de1c-107">Properties</span></span>
| <span data-ttu-id="4de1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4de1c-108">Property</span></span>     | <span data-ttu-id="4de1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4de1c-109">Type</span></span>   |<span data-ttu-id="4de1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de1c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4de1c-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="4de1c-111">automaticReplies</span></span> | [<span data-ttu-id="4de1c-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="4de1c-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="4de1c-113">Dicas para a resposta automática de email se ele foi configurado pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="4de1c-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="4de1c-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="4de1c-114">customMailTip</span></span> | <span data-ttu-id="4de1c-115">String</span><span class="sxs-lookup"><span data-stu-id="4de1c-115">String</span></span> | <span data-ttu-id="4de1c-116">Uma dica de email personalizado que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="4de1c-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="4de1c-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="4de1c-117">deliveryRestricted</span></span>| <span data-ttu-id="4de1c-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="4de1c-118">Boolean</span></span> | <span data-ttu-id="4de1c-119">Se caixa de correio do destinatário é restrita, por exemplo, aceitar mensagens de apenas uma lista de remetentes confiáveis, predefinida rejeitar mensagens de uma lista de remetentes predefinida, ou aceitar mensagens de apenas os remetentes autenticados.</span><span class="sxs-lookup"><span data-stu-id="4de1c-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="4de1c-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4de1c-120">emailAddress</span></span> | [<span data-ttu-id="4de1c-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4de1c-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="4de1c-122">O endereço de email do destinatário para obter dicas de email para.</span><span class="sxs-lookup"><span data-stu-id="4de1c-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="4de1c-123">erro</span><span class="sxs-lookup"><span data-stu-id="4de1c-123">error</span></span> | [<span data-ttu-id="4de1c-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="4de1c-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="4de1c-125">Erros que ocorrem durante a ação [getMailTips](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="4de1c-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="4de1c-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="4de1c-126">externalMemberCount</span></span> | <span data-ttu-id="4de1c-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4de1c-127">Int32</span></span> | <span data-ttu-id="4de1c-128">O número de membros externos se o destinatário é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4de1c-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="4de1c-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="4de1c-129">isModerated</span></span> |<span data-ttu-id="4de1c-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="4de1c-130">Boolean</span></span>  | <span data-ttu-id="4de1c-131">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="4de1c-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="4de1c-132">Por exemplo, se o destinatário é uma lista de distribuição grandes e um moderador tiver sido definido até aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário requer aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="4de1c-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="4de1c-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="4de1c-133">mailboxFull</span></span> | <span data-ttu-id="4de1c-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="4de1c-134">Boolean</span></span> | <span data-ttu-id="4de1c-135">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="4de1c-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="4de1c-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="4de1c-136">maxMessageSize</span></span> | <span data-ttu-id="4de1c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4de1c-137">Int32</span></span> | <span data-ttu-id="4de1c-138">O tamanho máximo da mensagem que tenha sido configurado para a organização ou a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="4de1c-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="4de1c-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="4de1c-139">recipientScope</span></span> | <span data-ttu-id="4de1c-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="4de1c-140">recipientScopeType</span></span> | <span data-ttu-id="4de1c-141">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="4de1c-141">The scope of the recipient.</span></span> <span data-ttu-id="4de1c-142">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="4de1c-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="4de1c-143">Por exemplo, um administrador pode definir outra organização seja seu parceiro de"".</span><span class="sxs-lookup"><span data-stu-id="4de1c-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="4de1c-144">O escopo é útil quando um administrador deseja que seja acessível a determinados escopos determinadas dicas de email.</span><span class="sxs-lookup"><span data-stu-id="4de1c-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="4de1c-145">Também é útil para remetentes para informar a eles que seus mensagem pode deixar a organização, ajudando-os a tomar as decisões corretas sobre palavras, o tom e o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4de1c-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="4de1c-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="4de1c-146">recipientSuggestions</span></span> | <span data-ttu-id="4de1c-147">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="4de1c-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="4de1c-148">Destinatários sugerido contextos de anteriores com base em onde eles aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="4de1c-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="4de1c-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="4de1c-149">totalMemberCount</span></span> | <span data-ttu-id="4de1c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4de1c-150">Int32</span></span> | <span data-ttu-id="4de1c-151">O número de membros se o destinatário é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4de1c-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="4de1c-152">valores de recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="4de1c-152">recipientScopeType values</span></span>

| <span data-ttu-id="4de1c-153">Valor</span><span class="sxs-lookup"><span data-stu-id="4de1c-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="4de1c-154">nenhum</span><span class="sxs-lookup"><span data-stu-id="4de1c-154">none</span></span>
| <span data-ttu-id="4de1c-155">interno</span><span class="sxs-lookup"><span data-stu-id="4de1c-155">internal</span></span>
| <span data-ttu-id="4de1c-156">externo</span><span class="sxs-lookup"><span data-stu-id="4de1c-156">external</span></span>
| <span data-ttu-id="4de1c-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="4de1c-157">externalPartner</span></span>
| <span data-ttu-id="4de1c-158">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="4de1c-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="4de1c-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4de1c-159">JSON representation</span></span>

<span data-ttu-id="4de1c-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4de1c-160">Here is a JSON representation of the resource.</span></span>

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

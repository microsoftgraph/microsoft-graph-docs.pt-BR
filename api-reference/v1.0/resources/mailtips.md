---
title: tipo de recurso dicas de texto
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem de ausência temporária '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 90f6f1a66631223a45a34797b6d18c13259d6241
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036320"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="23792-104">tipo de recurso dicas de texto</span><span class="sxs-lookup"><span data-stu-id="23792-104">mailTips resource type</span></span>

<span data-ttu-id="23792-105">Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="23792-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="23792-106">Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.</span><span class="sxs-lookup"><span data-stu-id="23792-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="23792-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23792-107">Properties</span></span>
| <span data-ttu-id="23792-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23792-108">Property</span></span>     | <span data-ttu-id="23792-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="23792-109">Type</span></span>   |<span data-ttu-id="23792-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23792-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23792-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="23792-111">automaticReplies</span></span> | [<span data-ttu-id="23792-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="23792-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="23792-113">Dicas de email para resposta automática se tiver sido configurada pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="23792-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="23792-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="23792-114">customMailTip</span></span> | <span data-ttu-id="23792-115">String</span><span class="sxs-lookup"><span data-stu-id="23792-115">String</span></span> | <span data-ttu-id="23792-116">Uma dica de email personalizada que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="23792-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="23792-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="23792-117">deliveryRestricted</span></span>| <span data-ttu-id="23792-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="23792-118">Boolean</span></span> | <span data-ttu-id="23792-119">Se a caixa de correio do destinatário é restrita, por exemplo, aceitando mensagens de apenas uma lista predefinida de remetentes, rejeitando mensagens de uma lista predefinida de remetentes ou aceitando mensagens de somente remetentes autenticados.</span><span class="sxs-lookup"><span data-stu-id="23792-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="23792-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="23792-120">emailAddress</span></span> | [<span data-ttu-id="23792-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="23792-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="23792-122">O endereço de email do destinatário para o qual obter dicas de email.</span><span class="sxs-lookup"><span data-stu-id="23792-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="23792-123">erro</span><span class="sxs-lookup"><span data-stu-id="23792-123">error</span></span> | [<span data-ttu-id="23792-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="23792-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="23792-125">Erros que ocorrem durante a [](../api/user-getmailtips.md) ação comdicas de as.</span><span class="sxs-lookup"><span data-stu-id="23792-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="23792-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="23792-126">externalMemberCount</span></span> | <span data-ttu-id="23792-127">Int32</span><span class="sxs-lookup"><span data-stu-id="23792-127">Int32</span></span> | <span data-ttu-id="23792-128">O número de membros externos se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="23792-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="23792-129">ismoderadod</span><span class="sxs-lookup"><span data-stu-id="23792-129">isModerated</span></span> |<span data-ttu-id="23792-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="23792-130">Boolean</span></span>  | <span data-ttu-id="23792-131">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="23792-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="23792-132">Por exemplo, se o destinatário for uma lista de distribuição grande e um moderador tiver sido configurado para aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens a um destinatário exigir a aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="23792-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="23792-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="23792-133">mailboxFull</span></span> | <span data-ttu-id="23792-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="23792-134">Boolean</span></span> | <span data-ttu-id="23792-135">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="23792-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="23792-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="23792-136">maxMessageSize</span></span> | <span data-ttu-id="23792-137">Int32</span><span class="sxs-lookup"><span data-stu-id="23792-137">Int32</span></span> | <span data-ttu-id="23792-138">O tamanho máximo da mensagem que foi configurada para a organização ou caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="23792-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="23792-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="23792-139">recipientScope</span></span> | <span data-ttu-id="23792-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="23792-140">recipientScopeType</span></span> | <span data-ttu-id="23792-141">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="23792-141">The scope of the recipient.</span></span> <span data-ttu-id="23792-142">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="23792-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="23792-143">Por exemplo, um administrador pode definir outra organização como "parceiro".</span><span class="sxs-lookup"><span data-stu-id="23792-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="23792-144">O escopo será útil se um administrador quiser que determinadas dicas de usuários fiquem acessíveis para determinados escopos.</span><span class="sxs-lookup"><span data-stu-id="23792-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="23792-145">Também é útil para os remetentes informar que a mensagem pode sair da organização, ajudando-os a tomar as decisões corretas sobre o texto, o Tom e o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="23792-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="23792-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="23792-146">recipientSuggestions</span></span> | <span data-ttu-id="23792-147">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="23792-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="23792-148">Os destinatários sugeridos com base em contextos anteriores, onde aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="23792-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="23792-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="23792-149">totalMemberCount</span></span> | <span data-ttu-id="23792-150">Int32</span><span class="sxs-lookup"><span data-stu-id="23792-150">Int32</span></span> | <span data-ttu-id="23792-151">O número de membros se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="23792-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="23792-152">valores de recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="23792-152">recipientScopeType values</span></span>

| <span data-ttu-id="23792-153">Valor</span><span class="sxs-lookup"><span data-stu-id="23792-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="23792-154">none</span><span class="sxs-lookup"><span data-stu-id="23792-154">none</span></span>
| <span data-ttu-id="23792-155">internamente</span><span class="sxs-lookup"><span data-stu-id="23792-155">internal</span></span>
| <span data-ttu-id="23792-156">externo</span><span class="sxs-lookup"><span data-stu-id="23792-156">external</span></span>
| <span data-ttu-id="23792-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="23792-157">externalPartner</span></span>
| <span data-ttu-id="23792-158">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="23792-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="23792-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23792-159">JSON representation</span></span>

<span data-ttu-id="23792-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23792-160">Here is a JSON representation of the resource.</span></span>

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

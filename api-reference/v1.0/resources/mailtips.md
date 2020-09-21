---
title: tipo de recurso dicas de texto
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem de ausência temporária '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bf331b0263027008923698c642a2ddec7464e53e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965544"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="9ba6a-104">tipo de recurso dicas de texto</span><span class="sxs-lookup"><span data-stu-id="9ba6a-104">mailTips resource type</span></span>

<span data-ttu-id="9ba6a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ba6a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ba6a-106">Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="9ba6a-107">Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="9ba6a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ba6a-108">Properties</span></span>
| <span data-ttu-id="9ba6a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ba6a-109">Property</span></span>     | <span data-ttu-id="9ba6a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ba6a-110">Type</span></span>   |<span data-ttu-id="9ba6a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ba6a-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ba6a-112">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="9ba6a-112">automaticReplies</span></span> | [<span data-ttu-id="9ba6a-113">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="9ba6a-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="9ba6a-114">Dicas de email para resposta automática se tiver sido configurada pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="9ba6a-115">customMailTip</span><span class="sxs-lookup"><span data-stu-id="9ba6a-115">customMailTip</span></span> | <span data-ttu-id="9ba6a-116">String</span><span class="sxs-lookup"><span data-stu-id="9ba6a-116">String</span></span> | <span data-ttu-id="9ba6a-117">Uma dica de email personalizada que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="9ba6a-118">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="9ba6a-118">deliveryRestricted</span></span>| <span data-ttu-id="9ba6a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba6a-119">Boolean</span></span> | <span data-ttu-id="9ba6a-120">Se a caixa de correio do destinatário é restrita, por exemplo, aceitando mensagens de apenas uma lista predefinida de remetentes, rejeitando mensagens de uma lista predefinida de remetentes ou aceitando mensagens de somente remetentes autenticados.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="9ba6a-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9ba6a-121">emailAddress</span></span> | [<span data-ttu-id="9ba6a-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9ba6a-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="9ba6a-123">O endereço de email do destinatário para o qual obter dicas de email.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="9ba6a-124">erro</span><span class="sxs-lookup"><span data-stu-id="9ba6a-124">error</span></span> | [<span data-ttu-id="9ba6a-125">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="9ba6a-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="9ba6a-126">Erros que ocorrem durante a ação [comdicas](../api/user-getmailtips.md) de as.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="9ba6a-127">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="9ba6a-127">externalMemberCount</span></span> | <span data-ttu-id="9ba6a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba6a-128">Int32</span></span> | <span data-ttu-id="9ba6a-129">O número de membros externos se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="9ba6a-130">ismoderadod</span><span class="sxs-lookup"><span data-stu-id="9ba6a-130">isModerated</span></span> |<span data-ttu-id="9ba6a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba6a-131">Boolean</span></span>  | <span data-ttu-id="9ba6a-132">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="9ba6a-133">Por exemplo, se o destinatário for uma lista de distribuição grande e um moderador tiver sido configurado para aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens a um destinatário exigir a aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="9ba6a-134">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="9ba6a-134">mailboxFull</span></span> | <span data-ttu-id="9ba6a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba6a-135">Boolean</span></span> | <span data-ttu-id="9ba6a-136">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="9ba6a-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="9ba6a-137">maxMessageSize</span></span> | <span data-ttu-id="9ba6a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba6a-138">Int32</span></span> | <span data-ttu-id="9ba6a-139">O tamanho máximo da mensagem que foi configurada para a organização ou caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="9ba6a-140">recipientScope</span><span class="sxs-lookup"><span data-stu-id="9ba6a-140">recipientScope</span></span> | <span data-ttu-id="9ba6a-141">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="9ba6a-141">recipientScopeType</span></span> | <span data-ttu-id="9ba6a-142">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-142">The scope of the recipient.</span></span> <span data-ttu-id="9ba6a-143">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="9ba6a-144">Por exemplo, um administrador pode definir outra organização como "parceiro".</span><span class="sxs-lookup"><span data-stu-id="9ba6a-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="9ba6a-145">O escopo será útil se um administrador quiser que determinadas dicas de usuários fiquem acessíveis para determinados escopos.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="9ba6a-146">Também é útil para os remetentes informar que a mensagem pode sair da organização, ajudando-os a tomar as decisões corretas sobre o texto, o Tom e o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="9ba6a-147">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="9ba6a-147">recipientSuggestions</span></span> | <span data-ttu-id="9ba6a-148">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9ba6a-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="9ba6a-149">Os destinatários sugeridos com base em contextos anteriores, onde aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="9ba6a-150">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="9ba6a-150">totalMemberCount</span></span> | <span data-ttu-id="9ba6a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba6a-151">Int32</span></span> | <span data-ttu-id="9ba6a-152">O número de membros se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-152">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="9ba6a-153">valores de recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="9ba6a-153">recipientScopeType values</span></span>

| <span data-ttu-id="9ba6a-154">Valor</span><span class="sxs-lookup"><span data-stu-id="9ba6a-154">Value</span></span>
|:-------------------------
| <span data-ttu-id="9ba6a-155">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9ba6a-155">none</span></span>
| <span data-ttu-id="9ba6a-156">internamente</span><span class="sxs-lookup"><span data-stu-id="9ba6a-156">internal</span></span>
| <span data-ttu-id="9ba6a-157">externo</span><span class="sxs-lookup"><span data-stu-id="9ba6a-157">external</span></span>
| <span data-ttu-id="9ba6a-158">externalPartner</span><span class="sxs-lookup"><span data-stu-id="9ba6a-158">externalPartner</span></span>
| <span data-ttu-id="9ba6a-159">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="9ba6a-159">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="9ba6a-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ba6a-160">JSON representation</span></span>

<span data-ttu-id="9ba6a-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ba6a-161">Here is a JSON representation of the resource.</span></span>

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


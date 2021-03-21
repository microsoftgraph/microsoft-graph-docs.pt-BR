---
title: Tipo de recurso mailTips
description: 'Mensagens informativas sobre um destinatário, que são exibidas para os usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem fora do escritório '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0be2ee10807dadd4c8bd32dcec438f001fe8d481
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960415"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="b81c6-104">Tipo de recurso mailTips</span><span class="sxs-lookup"><span data-stu-id="b81c6-104">mailTips resource type</span></span>

<span data-ttu-id="b81c6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b81c6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b81c6-106">Mensagens informativas sobre um destinatário, que são exibidas para os usuários enquanto eles compõem uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b81c6-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="b81c6-107">Por exemplo, uma mensagem fora do escritório como uma resposta automática para um destinatário de mensagem.</span><span class="sxs-lookup"><span data-stu-id="b81c6-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="b81c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b81c6-108">Properties</span></span>
| <span data-ttu-id="b81c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b81c6-109">Property</span></span>     | <span data-ttu-id="b81c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b81c6-110">Type</span></span>   |<span data-ttu-id="b81c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b81c6-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b81c6-112">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="b81c6-112">automaticReplies</span></span> | [<span data-ttu-id="b81c6-113">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="b81c6-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="b81c6-114">Dicas de email para resposta automática se ela tiver sido configurada pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="b81c6-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="b81c6-115">customMailTip</span><span class="sxs-lookup"><span data-stu-id="b81c6-115">customMailTip</span></span> | <span data-ttu-id="b81c6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b81c6-116">String</span></span> | <span data-ttu-id="b81c6-117">Uma dica de email personalizada que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b81c6-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="b81c6-118">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="b81c6-118">deliveryRestricted</span></span>| <span data-ttu-id="b81c6-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="b81c6-119">Boolean</span></span> | <span data-ttu-id="b81c6-120">Se a caixa de correio do destinatário é restrita, por exemplo, aceitar mensagens de apenas uma lista predefinida de destinatários, rejeitar mensagens de uma lista predefinida de destinatários ou aceitar mensagens apenas de destinatários autenticados.</span><span class="sxs-lookup"><span data-stu-id="b81c6-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="b81c6-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b81c6-121">emailAddress</span></span> | [<span data-ttu-id="b81c6-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b81c6-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="b81c6-123">O endereço de email do destinatário para o que receber dicas de email.</span><span class="sxs-lookup"><span data-stu-id="b81c6-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="b81c6-124">erro</span><span class="sxs-lookup"><span data-stu-id="b81c6-124">error</span></span> | [<span data-ttu-id="b81c6-125">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="b81c6-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="b81c6-126">Erros que ocorrem durante a [ação getMailTips.](../api/user-getmailtips.md)</span><span class="sxs-lookup"><span data-stu-id="b81c6-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="b81c6-127">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="b81c6-127">externalMemberCount</span></span> | <span data-ttu-id="b81c6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b81c6-128">Int32</span></span> | <span data-ttu-id="b81c6-129">O número de membros externos se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b81c6-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="b81c6-130">isModerated</span><span class="sxs-lookup"><span data-stu-id="b81c6-130">isModerated</span></span> |<span data-ttu-id="b81c6-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="b81c6-131">Boolean</span></span>  | <span data-ttu-id="b81c6-132">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="b81c6-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="b81c6-133">Por exemplo, se o destinatário for uma lista de distribuição grande e um moderador tiver sido definido para aprovar mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário exigir aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b81c6-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="b81c6-134">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="b81c6-134">mailboxFull</span></span> | <span data-ttu-id="b81c6-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="b81c6-135">Boolean</span></span> | <span data-ttu-id="b81c6-136">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b81c6-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="b81c6-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="b81c6-137">maxMessageSize</span></span> | <span data-ttu-id="b81c6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b81c6-138">Int32</span></span> | <span data-ttu-id="b81c6-139">O tamanho máximo da mensagem que foi configurado para a organização ou a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b81c6-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="b81c6-140">recipientScope</span><span class="sxs-lookup"><span data-stu-id="b81c6-140">recipientScope</span></span> | <span data-ttu-id="b81c6-141">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="b81c6-141">recipientScopeType</span></span> | <span data-ttu-id="b81c6-142">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b81c6-142">The scope of the recipient.</span></span> <span data-ttu-id="b81c6-143">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="b81c6-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="b81c6-144">Por exemplo, um administrador pode definir outra organização como seu "parceiro".</span><span class="sxs-lookup"><span data-stu-id="b81c6-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="b81c6-145">O escopo será útil se um administrador quiser que determinadas dicas de email sejam acessíveis a determinados escopos.</span><span class="sxs-lookup"><span data-stu-id="b81c6-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="b81c6-146">Também é útil para os envios informá-los de que sua mensagem pode sair da organização, ajudando-os a tomar as decisões corretas sobre texto, tom e conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b81c6-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="b81c6-147">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="b81c6-147">recipientSuggestions</span></span> | <span data-ttu-id="b81c6-148">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b81c6-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="b81c6-149">Destinatários sugeridos com base em contextos anteriores em que aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b81c6-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="b81c6-150">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="b81c6-150">totalMemberCount</span></span> | <span data-ttu-id="b81c6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b81c6-151">Int32</span></span> | <span data-ttu-id="b81c6-152">O número de membros se o destinatário for uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b81c6-152">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b81c6-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b81c6-153">JSON representation</span></span>

<span data-ttu-id="b81c6-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b81c6-154">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



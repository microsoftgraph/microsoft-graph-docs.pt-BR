---
title: tipo de recurso de dicas de email
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem. Por exemplo, uma mensagem de ausência temporária '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508409"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="7297b-104">tipo de recurso de dicas de email</span><span class="sxs-lookup"><span data-stu-id="7297b-104">mailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7297b-105">Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7297b-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="7297b-106">Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.</span><span class="sxs-lookup"><span data-stu-id="7297b-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="7297b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7297b-107">Properties</span></span>
| <span data-ttu-id="7297b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7297b-108">Property</span></span>     | <span data-ttu-id="7297b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7297b-109">Type</span></span>   |<span data-ttu-id="7297b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7297b-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7297b-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="7297b-111">automaticReplies</span></span> | [<span data-ttu-id="7297b-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="7297b-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="7297b-113">Dicas para a resposta automática de email se ele foi configurado pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="7297b-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="7297b-114">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="7297b-114">customMailTip</span></span> | <span data-ttu-id="7297b-115">String</span><span class="sxs-lookup"><span data-stu-id="7297b-115">String</span></span> | <span data-ttu-id="7297b-116">Uma dica de email personalizado que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="7297b-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="7297b-117">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="7297b-117">deliveryRestricted</span></span>| <span data-ttu-id="7297b-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="7297b-118">Boolean</span></span> | <span data-ttu-id="7297b-119">Se caixa de correio do destinatário é restrita, por exemplo, aceitar mensagens de apenas uma lista de remetentes confiáveis, predefinida rejeitar mensagens de uma lista de remetentes predefinida, ou aceitar mensagens de apenas os remetentes autenticados.</span><span class="sxs-lookup"><span data-stu-id="7297b-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="7297b-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7297b-120">emailAddress</span></span> | [<span data-ttu-id="7297b-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7297b-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="7297b-122">O endereço de email do destinatário para obter dicas de email para.</span><span class="sxs-lookup"><span data-stu-id="7297b-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="7297b-123">erro</span><span class="sxs-lookup"><span data-stu-id="7297b-123">error</span></span> | [<span data-ttu-id="7297b-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="7297b-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="7297b-125">Erros que ocorrem durante a ação [getMailTips](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="7297b-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="7297b-126">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="7297b-126">externalMemberCount</span></span> | <span data-ttu-id="7297b-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7297b-127">Int32</span></span> | <span data-ttu-id="7297b-128">O número de membros externos se o destinatário é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7297b-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="7297b-129">IsModerated</span><span class="sxs-lookup"><span data-stu-id="7297b-129">isModerated</span></span> |<span data-ttu-id="7297b-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="7297b-130">Boolean</span></span>  | <span data-ttu-id="7297b-131">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="7297b-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="7297b-132">Por exemplo, se o destinatário é uma lista de distribuição grandes e um moderador tiver sido definido até aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário requer aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="7297b-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="7297b-133">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="7297b-133">mailboxFull</span></span> | <span data-ttu-id="7297b-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="7297b-134">Boolean</span></span> | <span data-ttu-id="7297b-135">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="7297b-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="7297b-136">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="7297b-136">maxMessageSize</span></span> | <span data-ttu-id="7297b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7297b-137">Int32</span></span> | <span data-ttu-id="7297b-138">O tamanho máximo da mensagem que tenha sido configurado para a organização ou a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="7297b-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="7297b-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="7297b-139">recipientScope</span></span> | <span data-ttu-id="7297b-140">String</span><span class="sxs-lookup"><span data-stu-id="7297b-140">String</span></span> | <span data-ttu-id="7297b-141">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="7297b-141">The scope of the recipient.</span></span> <span data-ttu-id="7297b-142">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="7297b-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="7297b-143">Por exemplo, um administrador pode definir outra organização seja seu parceiro de"".</span><span class="sxs-lookup"><span data-stu-id="7297b-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="7297b-144">O escopo é útil quando um administrador deseja que seja acessível a determinados escopos determinadas dicas de email.</span><span class="sxs-lookup"><span data-stu-id="7297b-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="7297b-145">Também é útil para remetentes para informar a eles que seus mensagem pode deixar a organização, ajudando-os a tomar as decisões corretas sobre palavras, o tom e o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7297b-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="7297b-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="7297b-146">recipientSuggestions</span></span> | <span data-ttu-id="7297b-147">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7297b-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="7297b-148">Destinatários sugerido contextos de anteriores com base em onde eles aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7297b-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="7297b-149">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="7297b-149">totalMemberCount</span></span> | <span data-ttu-id="7297b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7297b-150">Int32</span></span> | <span data-ttu-id="7297b-151">O número de membros se o destinatário é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7297b-151">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7297b-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7297b-152">JSON representation</span></span>

<span data-ttu-id="7297b-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7297b-153">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

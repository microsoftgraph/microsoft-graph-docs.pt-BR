---
title: tipo de recurso de dicas de email
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem. Por exemplo, uma mensagem de ausência temporária '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed6d43e033b020b884a6cd1b6220b1ff566a507b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985953"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="ba4af-104">tipo de recurso de dicas de email</span><span class="sxs-lookup"><span data-stu-id="ba4af-104">mailTips resource type</span></span>

> <span data-ttu-id="ba4af-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ba4af-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba4af-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ba4af-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba4af-107">Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ba4af-107">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="ba4af-108">Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.</span><span class="sxs-lookup"><span data-stu-id="ba4af-108">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="ba4af-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba4af-109">Properties</span></span>
| <span data-ttu-id="ba4af-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba4af-110">Property</span></span>     | <span data-ttu-id="ba4af-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba4af-111">Type</span></span>   |<span data-ttu-id="ba4af-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba4af-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba4af-113">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="ba4af-113">automaticReplies</span></span> | [<span data-ttu-id="ba4af-114">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="ba4af-114">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="ba4af-115">Dicas para a resposta automática de email se ele foi configurado pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="ba4af-115">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="ba4af-116">customMailTip</span><span class="sxs-lookup"><span data-stu-id="ba4af-116">customMailTip</span></span> | <span data-ttu-id="ba4af-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-117">String</span></span> | <span data-ttu-id="ba4af-118">Uma dica de email personalizado que pode ser definida na caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ba4af-118">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="ba4af-119">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="ba4af-119">deliveryRestricted</span></span>| <span data-ttu-id="ba4af-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba4af-120">Boolean</span></span> | <span data-ttu-id="ba4af-121">Se caixa de correio do destinatário é restrita, por exemplo, aceitar mensagens de apenas uma lista de remetentes confiáveis, predefinida rejeitar mensagens de uma lista de remetentes predefinida, ou aceitar mensagens de apenas os remetentes autenticados.</span><span class="sxs-lookup"><span data-stu-id="ba4af-121">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="ba4af-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ba4af-122">emailAddress</span></span> | [<span data-ttu-id="ba4af-123">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ba4af-123">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="ba4af-124">O endereço de email do destinatário para obter dicas de email para.</span><span class="sxs-lookup"><span data-stu-id="ba4af-124">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="ba4af-125">erro</span><span class="sxs-lookup"><span data-stu-id="ba4af-125">error</span></span> | [<span data-ttu-id="ba4af-126">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="ba4af-126">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="ba4af-127">Erros que ocorrem durante a ação [getMailTips](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="ba4af-127">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="ba4af-128">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ba4af-128">externalMemberCount</span></span> | <span data-ttu-id="ba4af-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ba4af-129">Int32</span></span> | <span data-ttu-id="ba4af-130">O número de membros externos se o destinatário é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ba4af-130">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="ba4af-131">isModerated</span><span class="sxs-lookup"><span data-stu-id="ba4af-131">isModerated</span></span> |<span data-ttu-id="ba4af-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba4af-132">Boolean</span></span>  | <span data-ttu-id="ba4af-133">Se o envio de mensagens para o destinatário requer aprovação.</span><span class="sxs-lookup"><span data-stu-id="ba4af-133">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="ba4af-134">Por exemplo, se o destinatário é uma lista de distribuição grandes e um moderador tiver sido definido até aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário requer aprovação do gerente do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ba4af-134">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="ba4af-135">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="ba4af-135">mailboxFull</span></span> | <span data-ttu-id="ba4af-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba4af-136">Boolean</span></span> | <span data-ttu-id="ba4af-137">O status completo da caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ba4af-137">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="ba4af-138">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="ba4af-138">maxMessageSize</span></span> | <span data-ttu-id="ba4af-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ba4af-139">Int32</span></span> | <span data-ttu-id="ba4af-140">O tamanho máximo da mensagem que tenha sido configurado para a organização ou a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ba4af-140">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="ba4af-141">recipientScope</span><span class="sxs-lookup"><span data-stu-id="ba4af-141">recipientScope</span></span> | <span data-ttu-id="ba4af-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba4af-142">String</span></span> | <span data-ttu-id="ba4af-143">O escopo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ba4af-143">The scope of the recipient.</span></span> <span data-ttu-id="ba4af-144">Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="ba4af-144">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="ba4af-145">Por exemplo, um administrador pode definir outra organização seja seu parceiro de"".</span><span class="sxs-lookup"><span data-stu-id="ba4af-145">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="ba4af-146">O escopo é útil quando um administrador deseja que seja acessível a determinados escopos determinadas dicas de email.</span><span class="sxs-lookup"><span data-stu-id="ba4af-146">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="ba4af-147">Também é útil para remetentes para informar a eles que seus mensagem pode deixar a organização, ajudando-os a tomar as decisões corretas sobre palavras, o tom e o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ba4af-147">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="ba4af-148">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="ba4af-148">recipientSuggestions</span></span> | <span data-ttu-id="ba4af-149">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="ba4af-149">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="ba4af-150">Destinatários sugerido contextos de anteriores com base em onde eles aparecem na mesma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ba4af-150">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="ba4af-151">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ba4af-151">totalMemberCount</span></span> | <span data-ttu-id="ba4af-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ba4af-152">Int32</span></span> | <span data-ttu-id="ba4af-153">O número de membros se o destinatário é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ba4af-153">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba4af-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba4af-154">JSON representation</span></span>

<span data-ttu-id="ba4af-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba4af-155">Here is a JSON representation of the resource.</span></span>

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

---
title: Tipo de recurso chatMessagePolicyViolation
description: Representa uma violação de política em uma mensagem de chat. As violações de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP).
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9c65b6dd1d07db43286a8cf9923f4a94f0855b34
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582267"
---
# <a name="chatmessagepolicyviolation-resource-type"></a><span data-ttu-id="e0456-104">Tipo de recurso chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="e0456-104">chatMessagePolicyViolation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0456-105">Representa uma violação de política em uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="e0456-105">Represents a policy violation on a chat message.</span></span> <span data-ttu-id="e0456-106">As violações de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP).</span><span class="sxs-lookup"><span data-stu-id="e0456-106">Policy violations are typically set by a data loss prevention (DLP) application.</span></span> <span data-ttu-id="e0456-107">Os aplicativos DLP monitoram chats para mensagens que contêm dados que os usuários não devem enviar.</span><span class="sxs-lookup"><span data-stu-id="e0456-107">DLP applications monitor chats for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="e0456-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0456-108">Properties</span></span>

| <span data-ttu-id="e0456-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0456-109">Property</span></span>   | <span data-ttu-id="e0456-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0456-110">Type</span></span> |<span data-ttu-id="e0456-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0456-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0456-112">dlpAction</span><span class="sxs-lookup"><span data-stu-id="e0456-112">dlpAction</span></span>|<span data-ttu-id="e0456-113">**chatMessagePolicyViolationDlpActionType**</span><span class="sxs-lookup"><span data-stu-id="e0456-113">**chatMessagePolicyViolationDlpActionType**</span></span>|<span data-ttu-id="e0456-114">A ação realizada pelo provedor DLP na mensagem com conteúdo sensível.</span><span class="sxs-lookup"><span data-stu-id="e0456-114">The action taken by the DLP provider on the message with sensitive content.</span></span> <span data-ttu-id="e0456-115">Os valores com suporte são:</span><span class="sxs-lookup"><span data-stu-id="e0456-115">Supported values are:</span></span> <li><span data-ttu-id="e0456-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0456-116">None</span></span></li><li><span data-ttu-id="e0456-117">NotifySender - Informe o remetente da violação, mas permita que os leitores leiam a mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0456-117">NotifySender -- Inform the sender of the violation but allow readers to read the message.</span></span></li><li><span data-ttu-id="e0456-118">BlockAccess - Impedir que os leitores leiam a mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0456-118">BlockAccess -- Block readers from reading the message.</span></span></li><li><span data-ttu-id="e0456-119">BlockAccessExternal - Impedir que os usuários de fora da organização leiam a mensagem, permitindo que os usuários dentro da organização leiam a mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0456-119">BlockAccessExternal -- Block users outside the organization from reading the message, while allowing users within the organization to read the message.</span></span></li>|
|<span data-ttu-id="e0456-120">justificationText</span><span class="sxs-lookup"><span data-stu-id="e0456-120">justificationText</span></span>|<span data-ttu-id="e0456-121">string</span><span class="sxs-lookup"><span data-stu-id="e0456-121">string</span></span>|<span data-ttu-id="e0456-122">Texto de justificativa fornecido pelo remetente da mensagem ao se sobressuperar uma violação de política.</span><span class="sxs-lookup"><span data-stu-id="e0456-122">Justification text provided by the sender of the message when overriding a policy violation.</span></span>|
|<span data-ttu-id="e0456-123">policyTip</span><span class="sxs-lookup"><span data-stu-id="e0456-123">policyTip</span></span>|[<span data-ttu-id="e0456-124">chatMessagePolicyViolationPolicyTip</span><span class="sxs-lookup"><span data-stu-id="e0456-124">chatMessagePolicyViolationPolicyTip</span></span>](chatmessagepolicyviolationpolicytip.md)|<span data-ttu-id="e0456-125">Informações a ser exibidas ao remetente da mensagem sobre o motivo pelo qual a mensagem foi sinalizada como uma violação.</span><span class="sxs-lookup"><span data-stu-id="e0456-125">Information to display to the message sender about why the message was flagged as a violation.</span></span> |
|<span data-ttu-id="e0456-126">userAction</span><span class="sxs-lookup"><span data-stu-id="e0456-126">userAction</span></span>|<span data-ttu-id="e0456-127">**chatMessagePolicyViolationUserActionType**</span><span class="sxs-lookup"><span data-stu-id="e0456-127">**chatMessagePolicyViolationUserActionType**</span></span>|<span data-ttu-id="e0456-128">Indica a ação tomada pelo usuário em uma mensagem bloqueada pelo provedor DLP.</span><span class="sxs-lookup"><span data-stu-id="e0456-128">Indicates the action taken by the user on a message blocked by the DLP provider.</span></span> <span data-ttu-id="e0456-129">Os valores com suporte são:</span><span class="sxs-lookup"><span data-stu-id="e0456-129">Supported values are:</span></span> <li><span data-ttu-id="e0456-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0456-130">None</span></span></li><li><span data-ttu-id="e0456-131">Override</span><span class="sxs-lookup"><span data-stu-id="e0456-131">Override</span></span></li><li><span data-ttu-id="e0456-132">ReportFalsePositive</span><span class="sxs-lookup"><span data-stu-id="e0456-132">ReportFalsePositive</span></span></li><span data-ttu-id="e0456-133">Quando o provedor de DLP está atualizando a mensagem para bloquear conteúdos confidenciais, userAction não é necessário.</span><span class="sxs-lookup"><span data-stu-id="e0456-133">When the DLP provider is updating the message for blocking sensitive content, userAction is not required.</span></span>|
|<span data-ttu-id="e0456-134">verdictDetails</span><span class="sxs-lookup"><span data-stu-id="e0456-134">verdictDetails</span></span>|<span data-ttu-id="e0456-135">**chatMessagePolicyViolationVerdictDetailsType**</span><span class="sxs-lookup"><span data-stu-id="e0456-135">**chatMessagePolicyViolationVerdictDetailsType**</span></span>|<span data-ttu-id="e0456-136">Indica quais ações o remetente pode tomar em resposta à violação da política.</span><span class="sxs-lookup"><span data-stu-id="e0456-136">Indicates what actions the sender may take in response to the policy violation.</span></span> <span data-ttu-id="e0456-137">Os valores com suporte são:</span><span class="sxs-lookup"><span data-stu-id="e0456-137">Supported values are:</span></span> <li><span data-ttu-id="e0456-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0456-138">None</span></span></li><li><span data-ttu-id="e0456-139">AllowFalsePositiveOverride -- Permite que o remetente declare a políticaViolation como um erro no aplicativo DLP e suas regras e permita que os leitores vejam a mensagem novamente se a dlpAction a tiver ocultado.</span><span class="sxs-lookup"><span data-stu-id="e0456-139">AllowFalsePositiveOverride -- Allows the sender to declare the policyViolation to be an error in the DLP app and its rules, and allow readers to see the message again if the dlpAction had hidden it.</span></span></li><li><span data-ttu-id="e0456-140">AllowOverrideWithoutJustification -- permite que o remetente extravase a violação de DLP e permita que os leitores vejam a mensagem novamente se a dlpAction a tiver ocultado, sem a necessidade de fornecer uma explicação para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="e0456-140">AllowOverrideWithoutJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, without needing to provide an explanation for doing so.</span></span> </li><li><span data-ttu-id="e0456-141">AllowOverrideWithJustification -- Permite que o remetente extravase a violação de DLP e permita que os leitores vejam a mensagem novamente se a dlpAction a tiver ocultado, depois de fornecer uma explicação para isso.</span><span class="sxs-lookup"><span data-stu-id="e0456-141">AllowOverrideWithJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, after providing an explanation for doing so.</span></span></li><span data-ttu-id="e0456-142">AllowOverrideWithoutJustification e AllowOverrideWithJustification são mutuamente exclusivos.</span><span class="sxs-lookup"><span data-stu-id="e0456-142">AllowOverrideWithoutJustification and AllowOverrideWithJustification are mutually exclusive.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e0456-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0456-143">JSON representation</span></span>

<span data-ttu-id="e0456-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0456-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userAction",
    "justificationText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}-->

```json
{
  "dlpAction": "string",
  "justificationText": "string",
  "policyTip": {"@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"},
  "userAction": "string",
  "verdictDetails": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message policy violation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

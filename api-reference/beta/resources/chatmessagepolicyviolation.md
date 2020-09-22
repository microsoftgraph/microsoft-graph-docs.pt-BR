---
title: tipo de recurso chatMessagePolicyViolation
description: Representa uma violação de política em uma mensagem de chat. As violações de política normalmente são definidas por um aplicativo DLP (prevenção de perda de dados).
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 458e6440806ac57248bb87c6313d78b4845d647f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081954"
---
# <a name="chatmessagepolicyviolation-resource-type"></a><span data-ttu-id="0b4d6-104">tipo de recurso chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="0b4d6-104">chatMessagePolicyViolation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b4d6-105">Representa uma violação de política em uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-105">Represents a policy violation on a chat message.</span></span> <span data-ttu-id="0b4d6-106">As violações de política normalmente são definidas por um aplicativo DLP (prevenção de perda de dados).</span><span class="sxs-lookup"><span data-stu-id="0b4d6-106">Policy violations are typically set by a data loss prevention (DLP) application.</span></span> <span data-ttu-id="0b4d6-107">Os aplicativos DLP monitoram chats para mensagens que contêm dados que os usuários não devem enviar.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-107">DLP applications monitor chats for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="0b4d6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b4d6-108">Properties</span></span>

| <span data-ttu-id="0b4d6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b4d6-109">Property</span></span>   | <span data-ttu-id="0b4d6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b4d6-110">Type</span></span> |<span data-ttu-id="0b4d6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b4d6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b4d6-112">dlpAction</span><span class="sxs-lookup"><span data-stu-id="0b4d6-112">dlpAction</span></span>|<span data-ttu-id="0b4d6-113">**chatMessagePolicyViolationDlpActionType**</span><span class="sxs-lookup"><span data-stu-id="0b4d6-113">**chatMessagePolicyViolationDlpActionType**</span></span>|<span data-ttu-id="0b4d6-114">A ação executada pelo provedor de DLP na mensagem com conteúdo confidencial.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-114">The action taken by the DLP provider on the message with sensitive content.</span></span> <span data-ttu-id="0b4d6-115">Os valores compatíveis são:</span><span class="sxs-lookup"><span data-stu-id="0b4d6-115">Supported values are:</span></span> <li><span data-ttu-id="0b4d6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b4d6-116">None</span></span></li><li><span data-ttu-id="0b4d6-117">NotifySender--informe o remetente da violação, mas permita que os leitores leiam a mensagem.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-117">NotifySender -- Inform the sender of the violation but allow readers to read the message.</span></span></li><li><span data-ttu-id="0b4d6-118">BlockAccess--impede que os leitores leiam a mensagem.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-118">BlockAccess -- Block readers from reading the message.</span></span></li><li><span data-ttu-id="0b4d6-119">BlockAccessExternal--impede que os usuários de fora da organização leiam a mensagem, permitindo que os usuários dentro da organização leiam a mensagem.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-119">BlockAccessExternal -- Block users outside the organization from reading the message, while allowing users within the organization to read the message.</span></span></li>|
|<span data-ttu-id="0b4d6-120">justificationText</span><span class="sxs-lookup"><span data-stu-id="0b4d6-120">justificationText</span></span>|<span data-ttu-id="0b4d6-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b4d6-121">string</span></span>|<span data-ttu-id="0b4d6-122">Texto de justificativa fornecido pelo remetente da mensagem ao substituir uma violação de política.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-122">Justification text provided by the sender of the message when overriding a policy violation.</span></span>|
|<span data-ttu-id="0b4d6-123">policyTip</span><span class="sxs-lookup"><span data-stu-id="0b4d6-123">policyTip</span></span>|[<span data-ttu-id="0b4d6-124">chatMessagePolicyViolationPolicyTip</span><span class="sxs-lookup"><span data-stu-id="0b4d6-124">chatMessagePolicyViolationPolicyTip</span></span>](chatmessagepolicyviolationpolicytip.md)|<span data-ttu-id="0b4d6-125">Informações a serem exibidas para o remetente da mensagem sobre por que a mensagem foi sinalizada como uma violação.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-125">Information to display to the message sender about why the message was flagged as a violation.</span></span> |
|<span data-ttu-id="0b4d6-126">UserAction</span><span class="sxs-lookup"><span data-stu-id="0b4d6-126">userAction</span></span>|<span data-ttu-id="0b4d6-127">**chatMessagePolicyViolationUserActionType**</span><span class="sxs-lookup"><span data-stu-id="0b4d6-127">**chatMessagePolicyViolationUserActionType**</span></span>|<span data-ttu-id="0b4d6-128">Indica a ação executada pelo usuário em uma mensagem bloqueada pelo provedor de DLP.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-128">Indicates the action taken by the user on a message blocked by the DLP provider.</span></span> <span data-ttu-id="0b4d6-129">Os valores compatíveis são:</span><span class="sxs-lookup"><span data-stu-id="0b4d6-129">Supported values are:</span></span> <li><span data-ttu-id="0b4d6-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b4d6-130">None</span></span></li><li><span data-ttu-id="0b4d6-131">Override</span><span class="sxs-lookup"><span data-stu-id="0b4d6-131">Override</span></span></li><li><span data-ttu-id="0b4d6-132">ReportFalsePositive</span><span class="sxs-lookup"><span data-stu-id="0b4d6-132">ReportFalsePositive</span></span></li><span data-ttu-id="0b4d6-133">Quando o provedor de DLP está atualizando a mensagem para bloquear conteúdo confidencial, UserAction não é necessário.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-133">When the DLP provider is updating the message for blocking sensitive content, userAction is not required.</span></span>|
|<span data-ttu-id="0b4d6-134">verdictDetails</span><span class="sxs-lookup"><span data-stu-id="0b4d6-134">verdictDetails</span></span>|<span data-ttu-id="0b4d6-135">**chatMessagePolicyViolationVerdictDetailsType**</span><span class="sxs-lookup"><span data-stu-id="0b4d6-135">**chatMessagePolicyViolationVerdictDetailsType**</span></span>|<span data-ttu-id="0b4d6-136">Indica quais ações o remetente pode executar em resposta à violação da política.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-136">Indicates what actions the sender may take in response to the policy violation.</span></span> <span data-ttu-id="0b4d6-137">Os valores compatíveis são:</span><span class="sxs-lookup"><span data-stu-id="0b4d6-137">Supported values are:</span></span> <li><span data-ttu-id="0b4d6-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b4d6-138">None</span></span></li><li><span data-ttu-id="0b4d6-139">AllowFalsePositiveOverride – permite que o remetente declare o policyViolation para ser um erro no aplicativo DLP e suas regras e permitir que os leitores vejam a mensagem novamente se o dlpAction tivesse ocultado.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-139">AllowFalsePositiveOverride -- Allows the sender to declare the policyViolation to be an error in the DLP app and its rules, and allow readers to see the message again if the dlpAction had hidden it.</span></span></li><li><span data-ttu-id="0b4d6-140">AllowOverrideWithoutJustification – permite que o remetente fique superlado da violação de DLP e permita que os leitores vejam a mensagem novamente se o dlpAction tivesse ocultado, sem a necessidade de fornecer uma explicação para isso.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-140">AllowOverrideWithoutJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, without needing to provide an explanation for doing so.</span></span> </li><li><span data-ttu-id="0b4d6-141">AllowOverrideWithJustification – permite que o remetente fique superlado da violação de DLP e permita que os leitores vejam a mensagem novamente se o dlpAction tivesse ocultado, depois de fornecer uma explicação para isso.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-141">AllowOverrideWithJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, after providing an explanation for doing so.</span></span></li><span data-ttu-id="0b4d6-142">AllowOverrideWithoutJustification e AllowOverrideWithJustification são mutuamente exclusivos.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-142">AllowOverrideWithoutJustification and AllowOverrideWithJustification are mutually exclusive.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0b4d6-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b4d6-143">JSON representation</span></span>

<span data-ttu-id="0b4d6-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b4d6-144">The following is a JSON representation of the resource.</span></span>

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

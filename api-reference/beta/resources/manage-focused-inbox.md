---
title: Gerenciar a Caixa de Entrada Prioritária
description: 'A Caixa de Entrada Focada permite que você veja mensagens importantes na guia da Caixa de Entrada e o restante das mensagens da Caixa `Focused` de Entrada na `Other` guia. O sistema de classificação '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 8f69c23e62ef5face5932a4fc392952a7a62ab1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129377"
---
# <a name="manage-focused-inbox"></a><span data-ttu-id="75ef8-103">Gerenciar a Caixa de Entrada Prioritária</span><span class="sxs-lookup"><span data-stu-id="75ef8-103">Manage Focused Inbox</span></span>

<span data-ttu-id="75ef8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ef8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75ef8-p101">A caixa de entrada prioritária permite que você veja mensagens importantes na guia `Focused` da Caixa de Entrada e o restante das mensagens na guia `Other`. O sistema de classificação organiza inicialmente as mensagens da Caixa de Entrada de maneira padrão. Você pode corrigir e treinar o sistema ao longo do tempo por meio da interface do usuário ou programaticamente. Quanto mais você usar esse recurso, melhor o sistema poderá deduzir quais mensagens de entrada são importantes.</span><span class="sxs-lookup"><span data-stu-id="75ef8-p101">Focused Inbox allows you to view important messages in the `Focused` tab of the Inbox, and the rest of the Inbox messages in the `Other` tab. The classification system initially organizes Inbox messages in a default way. You can correct and train the system over time through the user interface or programmatically. The more you use it, the better the system can infer which incoming message as important.</span></span>

<span data-ttu-id="75ef8-p102">Em nível programático, a API REST da Caixa de Entrada Prioritária funciona nas mensagens do usuário especificado e oferece suporte a uma propriedade **inferenceClassification** para cada mensagem. Os valores possíveis são `Focused` e `Other`, que indicam se o usuário considera essa mensagem como, respectivamente, mais importante e menos importante. Para corrigir como o sistema classifica uma mensagem, [atualize a propriedade inferenceClassification dessa mensagem](../api/message-update.md). Com o passar do tempo, essas correções também treinarão o sistema de classificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="75ef8-p102">At the programmatic level, the Focused Inbox REST API works on the specified user's messages, and supports an **inferenceClassification** property for each message. The possible values are `Focused` and `Other`, which indicate whether the user considers that message as, respectively, more important and less important. To correct how the system classifies a message, [update the inferenceClassification property of that message](../api/message-update.md). Over time, these corrections also train the message classification system.</span></span>

<span data-ttu-id="75ef8-p103">A API REST da Caixa de Entrada Prioritária também permite criar substituições. Cada substituição, representada por uma instância de [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md), é uma instrução para o sistema de classificação sempre designar as mensagens de um remetente específico de maneira consistente (ou seja, sempre como "Prioritário" ou sempre como "Outros"), independentemente de qualquer abordagem aprendida anteriormente. Você pode [criar](../api/inferenceclassification-post-overrides.md), [listar](../api/inferenceclassification-list-overrides.md), [atualizar](../api/inferenceclassificationoverride-update.md) e [excluir](../api/inferenceclassificationoverride-delete.md) substituições para o usuário especificado. As substituições do usuário, se houver, são acessíveis em uma propriedade de navegação **inferenceClassification**, que é uma coleção de instâncias de **inferenceClassificationOverride**. Substituições permitem que um usuário tenha mais controle sobre a classificação de mensagens de entrada e desenvolvem maior confiabilidade do sistema de classificação.</span><span class="sxs-lookup"><span data-stu-id="75ef8-p103">The Focused Inbox REST API also lets you create overrides. Each override, represented by an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance, is an instruction for the classification system to always designate messages from a specific sender in a consistent way (i.e., always as "Focused" or always as "Other"), regardless of any previously learned approach. You can [create](../api/inferenceclassification-post-overrides.md), [list](../api/inferenceclassification-list-overrides.md), [update](../api/inferenceclassificationoverride-update.md) and [delete](../api/inferenceclassificationoverride-delete.md) overrides for the specified user. That user's overrides, if any, are accessible in an **inferenceClassification** navigation property, which is a collection of **inferenceClassificationOverride** instances. Overrides allow a user more control over the classification of incoming messages, and build greater trust of the classification system.</span></span>

<span data-ttu-id="75ef8-p104">Observe que o sistema de classificação aprende e aplica a classificação apenas a mensagens recebidas na Caixa de Entrada. As mensagens em outras pastas são classificadas como "Prioritário" por padrão. Configurar uma substituição afeta as mensagens futuras que chegarem na Caixa de Entrada. A substituição não modifica a propriedade **inferenceClassification** em mensagens existentes em qualquer pasta, incluindo a Caixa de Entrada.</span><span class="sxs-lookup"><span data-stu-id="75ef8-p104">Note that the classification system learns and applies classification only on incoming messages in the Inbox. Messages in other folders are by default "Focused". Setting up an override affects future messages arriving in the Inbox; the override doesn't modify the **inferenceClassification** property in existing messages in any folder including the Inbox.</span></span>

## <a name="focused-inbox-api"></a><span data-ttu-id="75ef8-120">API de Caixa de Entrada Prioritária</span><span class="sxs-lookup"><span data-stu-id="75ef8-120">Focused Inbox API</span></span>

<span data-ttu-id="75ef8-121">**Treinando o sistema de classificação de mensagens**</span><span class="sxs-lookup"><span data-stu-id="75ef8-121">**Training the message classification system**</span></span>

[<span data-ttu-id="75ef8-122">Atualizar a propriedade inferenceClassification de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="75ef8-122">Update the inferenceClassification property of a message</span></span>](../api/message-update.md)


<span data-ttu-id="75ef8-123">**Usar substituições para classificar consistentemente por remetente**</span><span class="sxs-lookup"><span data-stu-id="75ef8-123">**Using overrides to classify consistently per sender**</span></span>

<span data-ttu-id="75ef8-124">[Criar uma substituição para um remetente](../api/inferenceclassification-post-overrides.md)  |  [Listar todas as substituições de usuário](../api/inferenceclassification-list-overrides.md) |</span><span class="sxs-lookup"><span data-stu-id="75ef8-124">[Create an override for a sender](../api/inferenceclassification-post-overrides.md) | [List all user overrides](../api/inferenceclassification-list-overrides.md) |</span></span>

<span data-ttu-id="75ef8-125">[Atualizar uma substituição para um remetente](../api/inferenceclassificationoverride-update.md)  |  [Excluir uma substituição de remetente](../api/inferenceclassificationoverride-delete.md)</span><span class="sxs-lookup"><span data-stu-id="75ef8-125">[Update an override for a sender](../api/inferenceclassificationoverride-update.md) | [Delete a sender override](../api/inferenceclassificationoverride-delete.md)</span></span>



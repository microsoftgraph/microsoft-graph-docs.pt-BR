---
title: Tipo de recurso chatMessagePolicyViolationPolicyTip
description: Representa propriedades de uma dica de política em um objeto chatMessagePolicyViolation. As dicas de política fornecem ao remetente informações sobre a violação da política.
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4373475c4219c05b1bdf7ea741c0ed6526253d234da916e0760a3ed46fee3312
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169659"
---
# <a name="chatmessagepolicytip-resource-type"></a>Tipo de recurso chatMessagePolicyTip

Representa as propriedades de uma dica de política em um [objeto chatMessagePolicyViolation.](chatmessagepolicyviolation.md) As dicas de política fornecem ao remetente informações sobre a violação da política.
As dicas de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP) que observa mensagens que contêm dados que os usuários não devem enviar.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|complianceUrl|string|A URL que um usuário pode visitar para ler sobre as políticas de prevenção contra perda de dados da organização. (ou seja, políticas sobre o que os usuários não devem dizer nos chats)|
|generalText|string|Texto explicativo mostrado ao remetente da mensagem.|
|matchedConditionDescriptions|coleção de cadeias de caracteres|A lista de dados impróprios na mensagem detectada pelo aplicativo de prevenção contra perda de dados. Cada aplicativo DLP define suas próprias condições, exemplos incluem "Número do Cartão de Crédito" e "Número da Previdência Social".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->
```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

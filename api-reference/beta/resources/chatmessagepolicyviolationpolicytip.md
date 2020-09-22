---
title: tipo de recurso chatMessagePolicyViolationPolicyTip
description: Representa as propriedades de uma dica de política em um objeto chatMessagePolicyViolation. As dicas de política fornecem ao remetente informações sobre a violação da política.
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7a12afbd3ffb8eac75eb89b5d2bb5095fbd2ae98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081953"
---
# <a name="chatmessagepolicytip-resource-type"></a>tipo de recurso chatMessagePolicyTip

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as propriedades de uma dica de política em um objeto [chatMessagePolicyViolation](chatmessagepolicyviolation.md) . As dicas de política fornecem ao remetente informações sobre a violação da política.
As dicas de política são normalmente definidas por um aplicativo DLP (prevenção de perda de dados) que observa mensagens que contêm dados que os usuários não devem enviar.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|complianceUrl|cadeia de caracteres|A URL que um usuário pode visitar para ler sobre as políticas de prevenção de perda de dados da organização. (IE, políticas sobre o que os usuários não devem dizer nos chats)|
|generalText|cadeia de caracteres|Texto explicativo mostrado ao remetente da mensagem.|
|matchedConditionDescriptions|coleção de cadeias de caracteres|A lista de dados inadequados na mensagem que foi detectada pelo aplicativo prevenção de perda de dados. Cada aplicativo DLP define suas próprias condições, exemplos incluem "número do cartão de crédito" e "número do CPF".|

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

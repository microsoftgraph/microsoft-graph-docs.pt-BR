---
title: Tipo de recurso chatMessagePolicyViolationPolicyTip
description: Representa propriedades de uma dica de política em um objeto chatMessagePolicyViolation. As dicas de política fornecem ao remetente informações sobre a violação da política.
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 58b0a80a7e9a8864b13e36e2cef8355c46fd340d
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582741"
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

---
title: Tipo de recurso outOfOfficeSettings
description: Representa as informações de acesso ao telefone para uma reunião online.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13f826babea1e6f9448d1ecb9b8100baaf962b20
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896631"
---
# <a name="outofofficesettings-resource-type"></a>Tipo de recurso outOfOfficeSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações fora do escritório relacionadas à [presença](presence.md) de um usuário.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| mensagem           | String  | A mensagem fora do escritório que o usuário configurou no cliente Outlook (Respostas Automáticas (Sem Office)) ou o cliente Teams (Agendar sem escritório). |
| isOutOfOffice      | Boolean  | True se:</br><ul><li>Atualmente, ele está na janela de tempo fora do escritório configurada no Outlook ou Teams cliente.</li><li>Atualmente, há um evento no calendário do usuário marcado como Show as Out of Office</li></ul></br>Caso contrário, false. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.outOfOfficeSettings"
}-->
```json
{
  "message": "String",
  "isOutOfOffice": "Boolean"
}
```

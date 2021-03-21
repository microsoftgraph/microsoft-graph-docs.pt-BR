---
title: Tipo de recurso outOfOfficeSettings
description: Representa as informações de acesso ao telefone para uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 018852150ef833d8cb114892790f911b4aad8fe0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960370"
---
# <a name="outofofficesettings-resource-type"></a>Tipo de recurso outOfOfficeSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações fora do escritório relacionadas à [presença](presence.md) de um usuário.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| mensagem           | String  | A mensagem fora do escritório que o usuário configurou no cliente do Outlook (Respostas Automáticas (Sem Escritório)) ou no cliente do Teams (Agendamento sem escritório). |
| isOutOfOffice      | Booliano  | True se:</br><ul><li>Ele está atualmente na janela de tempo fora do escritório configurada no cliente do Outlook ou do Teams.</li><li>Atualmente, há um evento no calendário do usuário marcado como Show as Out of Office</li></ul></br>Caso contrário, false. |

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

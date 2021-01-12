---
title: Tipo de recurso outOfOfficeSettings
description: Representa informações de acesso telefônico para uma reunião online.
author: elvinyang-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e3e179ec752cfffc4ae4711d9fd0bc541f1506d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796716"
---
# <a name="outofofficesettings-resource-type"></a>Tipo de recurso outOfOfficeSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de fora do escritório relacionadas [à presença](presence.md) de um usuário.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| mensagem           | String  | A mensagem de saída que o usuário configurou no cliente do Outlook (Respostas Automáticas (Fora do Escritório)) ou no cliente do Teams (Agendamento de saída do escritório). |
| isOutOfOffice      | Boolean  | True se:</br><ul><li>Atualmente, ele está na janela de tempo de não escritório configurada no cliente do Outlook ou do Teams.</li><li>Atualmente, há um evento no calendário do usuário marcado como Show as Out of Office</li></ul></br>Caso contrário, false. |

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

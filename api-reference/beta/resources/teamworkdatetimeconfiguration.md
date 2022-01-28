---
title: Tipo de recurso teamworkDateTimeConfiguration
description: Representa detalhes de configuração de data e hora para um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 489c76f123124aa0b6d6023d5a21dbc780e88a13
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262247"
---
# <a name="teamworkdatetimeconfiguration-resource-type"></a>Tipo de recurso teamworkDateTimeConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de configuração de data e hora para um dispositivo Microsoft Teams habilitado [para uso.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dateFormat|Cadeia de caracteres|O formato de data do dispositivo.|
|officeHoursEndTime|TimeOfDay|A hora do dia em que o dispositivo está desligado.|
|officeHoursStartTime|TimeOfDay|A hora do dia em que o dispositivo está ligado.|
|timeFormat|Cadeia de caracteres|O formato de hora do dispositivo.|
|timeZone|Cadeia de caracteres|O fuso horário ao qual o horário de expediente se aplica.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDateTimeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDateTimeConfiguration",
  "dateFormat": "String",
  "officeHoursEndTime": "String (time of day)",
  "officeHoursStartTime": "String (time of day)",
  "timeFormat": "String",
  "timeZone": "String"
}
```


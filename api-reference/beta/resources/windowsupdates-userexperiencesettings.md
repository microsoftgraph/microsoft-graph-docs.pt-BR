---
title: Tipo de recurso userExperienceSettings
description: Configurações controlar a experiência de atualização do usuário em um dispositivo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a5d920d1618cb6d212baf0487a39960638859cef
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067227"
---
# <a name="userexperiencesettings-resource-type"></a>Tipo de recurso userExperienceSettings

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações controlar a experiência de atualização do usuário em um dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|daysUntilForcedReboot|Int32|Especifica o número de dias após a instalação de uma atualização, durante o qual o usuário do dispositivo pode controlar quando o dispositivo é reiniciado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.userExperienceSettings",
  "daysUntilForcedReboot": "Integer"
}
```


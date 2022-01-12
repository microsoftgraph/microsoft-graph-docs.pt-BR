---
title: Tipo de recurso rolloutSettings
description: Configurações controlar como o serviço implanta uma atualização ao longo do tempo.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 398bfdf0a33829f64a6b06de098cfc07a5df835e
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791998"
---
# <a name="rolloutsettings-resource-type"></a>Tipo de recurso rolloutSettings

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações controlar como o serviço implanta uma atualização ao longo do tempo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Data em que dispositivos na implantação começam a receber a atualização. Quando não estiver definida, a implantação será iniciada assim que os dispositivos são atribuídos.|
|devicesPerOffer|Int32| Especifica o número de dispositivos oferecidos ao mesmo tempo. Não tem efeito quando **endDateTime** é definido. Quando **endDateTime** e **devicesPerOffer** não estão definidos, todos os dispositivos na implantação são oferecidos conteúdo ao mesmo tempo.|
|durationBetweenOffers|String|Especifica a duração entre cada conjunto de dispositivos que estão sendo oferecidos a atualização. Tem efeito quando **endDateTime** ou **devicesPerOffer** são definidos. O valor padrão `P1D` é (1 dia).|
|endDateTime|DateTimeOffset|Especifica a data anterior à qual todos os dispositivos atualmente na implantação são oferecidos a atualização. Os dispositivos adicionados após essa data são oferecidos imediatamente. Quando **endDateTime** e **devicesPerOffer** não estão definidos, todos os dispositivos na implantação são oferecidos conteúdo ao mesmo tempo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.rolloutSettings",
  "startDateTime": "String",
  "durationBetweenOffers": "String",
  "endDateTime": "String (timestamp)",
  "devicesPerOffer": "Integer"
}
```


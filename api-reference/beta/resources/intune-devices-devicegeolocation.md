---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3c8251987dee0aadafdb88eebd9e29afbb5f76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784997"
---
# <a name="devicegeolocation-resource-type"></a>Tipo de recurso deviceGeoLocation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Localização do dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|Hora em que a localização foi registrada, em relação ao UTC|
|lastCollectedDateTime|DateTimeOffset|Hora em que a localização foi registrada, em relação ao UTC|
|longitude|Duplo|Coordenada de longitude da localização do dispositivo|
|latitude|Duplo|Coordenada de latitude da localização do dispositivo|
|altitude|Duplo|Altitude, especificada em metros acima do nível do mar|
|horizontalAccuracy|Duplo|Precisão da latitude e da longitude em metros|
|verticalAccuracy|Duplo|Precisão da altitude em metros|
|heading|Duplo|Direção em graus do norte verdadeiro|
|speed|Double|Velocidade na qual o dispositivo está viajando, em metros por segundo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```




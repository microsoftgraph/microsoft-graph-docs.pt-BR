---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69e097d433d774c3dd445c94cd29eb059292806f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091226"
---
# <a name="devicegeolocation-resource-type"></a>Tipo de recurso deviceGeoLocation

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Localização do dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|Hora em que a localização foi registrada, em relação ao UTC|
|longitude|Double|Coordenada de longitude da localização do dispositivo|
|latitude|Double|Coordenada de latitude da localização do dispositivo|
|altitude|Double|Altitude, especificada em metros acima do nível do mar|
|horizontalAccuracy|Double|Precisão da latitude e da longitude em metros|
|verticalAccuracy|Double|Precisão da altitude em metros|
|heading|Double|Direção em graus do norte verdadeiro|
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










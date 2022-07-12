---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dfd61a6bc89b75a9af4b70c6368107bb0709378a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729542"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Tipo de recurso deviceOperatingSystemSummary

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo do sistema operacional do dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|androidCount|Int32|Número da contagem de dispositivos Android.|
|iosCount|Int32|Número da contagem de dispositivo iOS.|
|macOSCount|Int32|Número da contagem de dispositivos Mac OS X.|
|windowsMobileCount|Int32|Número da contagem de dispositivos móveis Windows.|
|windowsCount|Int32|Número da contagem de dispositivos Windows.|
|unknownCount|Int32|Número da contagem de dispositivos desconhecidos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```






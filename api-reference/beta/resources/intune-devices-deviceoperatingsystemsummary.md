---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ccb18fa2f8ec1545530dca13a7ed9d59be5a7504
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539096"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Tipo de recurso deviceOperatingSystemSummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|androidDedicatedCount|Int32|Número de dispositivos Android dedicados.|
|androidDeviceAdminCount|Int32|Número de dispositivos Android de administrador de dispositivos.|
|androidFullyManagedCount|Int32|Número de dispositivos Android totalmente gerenciados.|
|androidWorkProfileCount|Int32|Número de dispositivos Android de perfil de trabalho.|

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
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024
}
```




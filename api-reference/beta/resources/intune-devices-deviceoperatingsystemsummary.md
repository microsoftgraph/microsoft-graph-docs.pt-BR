---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
ms.openlocfilehash: 13224e18f117f13a6f7c7090d1aa9cb2686350c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040912"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Tipo de recurso deviceOperatingSystemSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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






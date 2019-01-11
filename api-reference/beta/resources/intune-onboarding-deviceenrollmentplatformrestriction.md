---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 009485c2051c47209074ae8b938e6b1b06de9eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843859"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Tipo de recurso deviceEnrollmentPlatformRestriction

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Restrições de registro específicas de plataformas
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|platformBlocked|Booliano|Bloqueia o registro da plataforma|
|personalDeviceEnrollmentBlocked|Booliano|Bloqueia o registro de dispositivos de sua propriedade|
|osMinimumVersion|Cadeia de caracteres|Versão do SO mínimo compatível|
|osMaximumVersion|Cadeia de caracteres|Versão do SO máximo compatível|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```






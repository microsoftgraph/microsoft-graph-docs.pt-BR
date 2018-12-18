---
title: tipo de recurso de deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: tfitzmac
ms.openlocfilehash: 01e0877388391deaebbda18e48247f4e3585a63a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316776"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>tipo de recurso de deviceManagementExchangeDeviceClass

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Classe de dispositivo no Exchange.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|String|Nome da classe do dispositivo que será afetada por essa regra.|
|type|[deviceManagementExchangeAccessRuleType](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|Tipo de dispositivo que é afetado por esta regra modelar p. ex., família. Os valores possíveis são: `family`, `model`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```






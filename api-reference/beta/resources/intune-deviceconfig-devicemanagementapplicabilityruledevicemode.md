---
title: Tipo de recurso deviceManagementApplicabilityRuleDeviceMode
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d880196154568862ed56d5cb887108eedc0325d2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818790"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a>Tipo de recurso deviceManagementApplicabilityRuleDeviceMode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceMode|[windows10DeviceModeType](../resources/intune-deviceconfig-windows10devicemodetype.md)|Regra de aplicabilidade para o modo de dispositivo. Os valores possíveis são: `standardConfiguration` e `sModeConfiguration`.|
|nome|Cadeia de caracteres|Nome do objeto.|
|ruleType|[deviceManagementApplicabilityRuleType](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|Tipo de regra de aplicabilidade. Os valores possíveis são: `include`, `exclude`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
  "deviceMode": "String",
  "name": "String",
  "ruleType": "String"
}
```




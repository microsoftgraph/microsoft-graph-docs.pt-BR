---
title: tipo de recurso deviceManagementApplicabilityRuleOsVersion
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 460618d844a01fc913e80022235f38b017091236
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469272"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a>tipo de recurso deviceManagementApplicabilityRuleOsVersion

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|minOSVersion|String|Versão mínima do sistema operacional para regra de aplicabilidade.|
|maxOSVersion|String|Versão do sistema operacional máximo para a regra de aplicabilidade.|
|nome|String|Nome do objeto.|
|ruleType|[deviceManagementApplicabilityRuleType](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|Tipo de regra de aplicabilidade. Os valores possíveis são: `include`, `exclude`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```




---
title: tipo de recurso deviceHealthScriptComplianceRule
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371451"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a>tipo de recurso deviceHealthScriptComplianceRule

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Detecção|[deviceHealthScriptDetectionType](../resources/intune-devices-devicehealthscriptdetectiontype.md)|Ainda não documentado. Os valores possíveis são: `notConfigured` e `string`.|
|operator|[deviceHealthScriptComplianceRuleOperator](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|Ainda não documentado. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`.|
|detecçaovalue|String|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




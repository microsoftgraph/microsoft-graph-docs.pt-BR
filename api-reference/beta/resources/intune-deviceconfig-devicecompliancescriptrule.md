---
title: tipo de recurso deviceComplianceScriptRule
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c524202b8e15d077895c47c1c66256d58ca2c3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789295"
---
# <a name="devicecompliancescriptrule-resource-type"></a>tipo de recurso deviceComplianceScriptRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingName|Cadeia de caracteres|Nome da configuração especificado na regra.|
|operator|[operador](../resources/intune-deviceconfig-operator.md)|Operador especificado na regra. Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` , `notContains` , `allOf` , `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` ,,,,,.|
|dataType|[Alinha](../resources/intune-deviceconfig-datatype.md)|Tipo de dados especificado na regra. Os valores possíveis são:, `none` `boolean` , `int64` , `double` , `string` , `dateTime` , `version` , `base64` , `xml` , `booleanArray` , `int64Array` , `doubleArray` ,, `stringArray` `dateTimeArray` `versionArray` .|
|normaliza|String|Operando especificado na regra.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "dataType": "String",
  "operand": "String"
}
```




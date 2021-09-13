---
title: Tipo de recurso deviceHealthScriptStringParameter
description: Propriedades do parâmetro de script String.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19a4c240b813e4dbbde5135179049c3c32a988f7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040152"
---
# <a name="devicehealthscriptstringparameter-resource-type"></a>Tipo de recurso deviceHealthScriptStringParameter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Propriedades do parâmetro de script String.


Herda de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|O nome do param Herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|description|Cadeia de caracteres|A descrição do param Herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|isRequired|Booliano|Se o param é necessário Herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|applyDefaultValueWhenNotAssigned|Boleano|Se aplicar DefaultValue quando não atribuído herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|defaultValue|Cadeia de Caracteres|O valor padrão do param de cadeia de caracteres|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptStringParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": "String"
}
```




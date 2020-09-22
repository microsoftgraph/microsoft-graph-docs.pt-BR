---
title: tipo de recurso deviceHealthScriptParameter
description: Propriedades básicas do parâmetro script.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad82da1915702448a62c0c99f6933ddf1a51c5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060297"
---
# <a name="devicehealthscriptparameter-resource-type"></a>tipo de recurso deviceHealthScriptParameter

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Propriedades básicas do parâmetro script.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|Cadeia de caracteres|O nome do parâmetro|
|description|String|A descrição do parâmetro|
|isRequired|Booliano|Se o parâmetro é obrigatório|
|applyDefaultValueWhenNotAssigned|Booliano|Se aplicar DefaultValue quando não atribuído|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true
}
```







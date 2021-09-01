---
title: Tipo de recurso deviceHealthScriptParameter
description: Propriedades base do parâmetro script.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ddfd8eb3d251060961429c511114a7ebc1dd7286
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793814"
---
# <a name="devicehealthscriptparameter-resource-type"></a>Tipo de recurso deviceHealthScriptParameter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Propriedades base do parâmetro script.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|O nome do param|
|descrição|Cadeia de caracteres|A descrição do param|
|isRequired|Booliano|Se o param é necessário|
|applyDefaultValueWhenNotAssigned|Boleano|Se aplicar DefaultValue quando não atribuído|

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




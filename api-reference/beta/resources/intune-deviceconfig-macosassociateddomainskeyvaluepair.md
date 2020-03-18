---
title: tipo de recurso macOSAssociatedDomainsKeyValuePair
description: Par chave de valor para domínios associados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a59f0566da2e2dffa64c059cc913923ec5cf58
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790318"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a>tipo de recurso macOSAssociatedDomainsKeyValuePair

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Par chave de valor para domínios associados


Herda de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Nome para este par chave-valor herdado de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)|
|value|Cadeia de caracteres|Valor para este par chave-valor herdado de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```




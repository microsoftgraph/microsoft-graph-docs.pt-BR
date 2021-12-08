---
title: Tipo de recurso keyLongValuePair
description: Par de valores longos da chave
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e3d0378b89bd1e05d33a1a7eabc54acaa11707cd
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347036"
---
# <a name="keylongvaluepair-resource-type"></a>Tipo de recurso keyLongValuePair

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Par de valores longos da chave

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Nome para esse par de valores longos de chave|
|valor|Int64|Valor para esse par de valores longos de chave|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyLongValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyLongValuePair",
  "name": "String",
  "value": 1024
}
```





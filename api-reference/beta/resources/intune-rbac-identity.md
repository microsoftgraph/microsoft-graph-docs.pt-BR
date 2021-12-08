---
title: tipo de recurso identity
description: A Identidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b689afec67cae4b0c228d1a3ee96498a87a2548e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346770"
---
# <a name="identity-resource-type"></a>tipo de recurso identity

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A Identidade

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador da identidade. Essa propriedade é somente leitura.|
|displayName|String|O nome de exibição da identidade. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identity",
  "id": "String (identifier)",
  "displayName": "String"
}
```





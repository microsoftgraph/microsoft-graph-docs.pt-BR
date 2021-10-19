---
title: Tipo de recurso bulkDriverActionResult
description: Um tipo complexo para representar o resultado da ação do driver em massa.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3332c2856968aa5ddcc7841a555f37ae9638496
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494945"
---
# <a name="bulkdriveractionresult-resource-type"></a>Tipo de recurso bulkDriverActionResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para representar o resultado da ação do driver em massa.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|successfulDriverIds|Coleção de cadeias de caracteres|Lista de IDs de driver onde a ação é bem-sucedida.|
|failedDriverIds|Coleção de cadeias de caracteres|Lista de IDs de driver onde a ação falhou.|
|notFoundDriverIds|Coleção de cadeias de caracteres|Lista de IDs de driver que não foram encontradas.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkDriverActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkDriverActionResult",
  "successfulDriverIds": [
    "String"
  ],
  "failedDriverIds": [
    "String"
  ],
  "notFoundDriverIds": [
    "String"
  ]
}
```




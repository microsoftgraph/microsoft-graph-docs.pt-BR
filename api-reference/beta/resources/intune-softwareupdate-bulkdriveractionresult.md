---
title: Tipo de recurso bulkDriverActionResult
description: Um tipo complexo para representar o resultado da ação do driver em massa.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db914be4405385199dc792120d9392fd79713ef1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342220"
---
# <a name="bulkdriveractionresult-resource-type"></a>Tipo de recurso bulkDriverActionResult

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para representar o resultado da ação do driver em massa.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|successfulDriverIds|Coleção String|Lista de IDs de driver onde a ação é bem-sucedida.|
|failedDriverIds|Coleção String|Lista de IDs de driver onde a ação falhou.|
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





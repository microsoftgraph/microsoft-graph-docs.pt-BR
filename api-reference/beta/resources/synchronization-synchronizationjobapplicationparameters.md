---
title: tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca91021ccb9fbc4cf8ec6c61b4edea979bb7c833
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523200"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>tipo de recurso synchronizationJobApplicationParameters

Namespace: microsoft.graph

Representa os objetos que serão provisionados e as regras de sincronização executadas. O recurso é usado principalmente para provisionamento sob demanda. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleId|String|O identificador de um synchronizationRule a ser aplicado.|
|olhos|coleção [synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobApplicationParameters",
  "ruleId": "String",
  "subjects": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```



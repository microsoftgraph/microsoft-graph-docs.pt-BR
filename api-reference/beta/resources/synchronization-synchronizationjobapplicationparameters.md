---
title: Tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2c17d67f766a398f94ab4962850a762fc62f6e53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133921"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Tipo de recurso synchronizationJobApplicationParameters

Namespace: microsoft.graph

Representa os objetos que serão provisionados e as regras de sincronização executadas. O recurso é usado principalmente para provisionamento sob demanda. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleId|String|O identificador de uma synchronizationRule a ser aplicada.|
|subjects|[Coleção synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.|

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



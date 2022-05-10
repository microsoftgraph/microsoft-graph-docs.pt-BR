---
title: Tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 08dc3f6494a2c7e641f6ebfc81eb223aa990eb69
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296448"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Tipo de recurso synchronizationJobApplicationParameters

Namespace: microsoft.graph

Representa os objetos que serão provisionados e as regras de sincronização executadas. O recurso é usado principalmente para provisionamento sob demanda. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleId|Cadeia de caracteres|O identificador do [synchronizationRule](synchronization-synchronizationrule.md) a ser aplicado. Essa ID de regra é definida no esquema [para um determinado trabalho ou modelo de sincronização](../api/synchronization-synchronizationschema-get.md). |
|Assuntos|[Coleção synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.|

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



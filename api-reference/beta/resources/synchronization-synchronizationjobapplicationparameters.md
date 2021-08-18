---
title: tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5d8ac5a51842d76f5c72eb2bba1d03fe1479eb30f57c498a1dcdb326f4c1ff51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224247"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>tipo de recurso synchronizationJobApplicationParameters

Namespace: microsoft.graph

Representa os objetos que serão provisionados e as regras de sincronização executadas. O recurso é usado principalmente para provisionamento sob demanda. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleId|Cadeia de caracteres|O identificador de uma sincronizaçãoRule a ser aplicada.|
|subjects|[coleção synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Os identificadores de um ou mais objetos aos quais um SynchronizationJob deve ser aplicado.|

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



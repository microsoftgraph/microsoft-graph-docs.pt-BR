---
title: tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 1f4de7d4c3d518b795d739a80403903842d16a16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090955"
---
# <a name="synchronizationjobsubject-resource-type"></a>tipo de recurso synchronizationJobSubject

Namespace: microsoft.graph

Representa os objetos que serão provisionados durante o provisionamento sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|objectId|Cadeia de caracteres|O identificador de um objeto ao qual um SynchronizationJob deve ser aplicado.|
|objectTypeName|Cadeia de Caracteres|O tipo do objeto ao qual um SynchronizationJob deve ser aplicado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String"
}
```



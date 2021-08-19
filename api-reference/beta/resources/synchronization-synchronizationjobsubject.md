---
title: tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c7dea31898cb0bfb521367042401be7c583c60c2868d4805682c9d0e707fc898
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226109"
---
# <a name="synchronizationjobsubject-resource-type"></a>tipo de recurso synchronizationJobSubject

Namespace: microsoft.graph

Representa os objetos que serão provisionados durante o provisionamento sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|objectId|Cadeia de caracteres|O identificador de um objeto ao qual um SynchronizationJob deve ser aplicado.|
|objectTypeName|Cadeia de caracteres|O tipo do objeto ao qual um SynchronizationJob deve ser aplicado.|

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



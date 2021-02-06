---
title: Tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c9e6d83ed7024556954740e89edcc18f7b56ba04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131995"
---
# <a name="synchronizationjobsubject-resource-type"></a>Tipo de recurso synchronizationJobSubject

Namespace: microsoft.graph

Representa os objetos que serão provisionados durante o provisionamento sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|objectId|Cadeia de caracteres|O identificador de um objeto ao qual um synchronizationJob deve ser aplicado.|
|objectTypeName|String|O tipo do objeto ao qual um synchronizationJob deve ser aplicado.|

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



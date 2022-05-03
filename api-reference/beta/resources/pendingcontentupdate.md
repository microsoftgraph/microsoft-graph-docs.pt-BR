---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está com a conclusão pendente.
ms.localizationpriority: medium
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: ec44c2c1d75bc11276d99dad1815c0d999b4f0e1
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176342"
---
# <a name="pendingcontentupdate-resource-type"></a>Tipo de recurso pendingContentUpdate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está pendente.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo         | Descrição |
|:-------------|:-------------|:------------|
|queuedDateTime|DateTimeOffset|Data e hora em que a operação binária pendente foi enfileirada no horário UTC. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->



---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está aguardando a conclusão.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1637ac3faa1d42cd47f49735a1b24fb60868a23d
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333383"
---
# <a name="pendingcontentupdate-resource-type"></a>tipo de recurso pendingContentUpdate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está aguardando a conclusão.

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

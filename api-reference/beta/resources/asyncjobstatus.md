---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 74ead4ca8e45c5baebe3ea74377ce102d9e2ee88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328533"
---
# <a name="asyncjobstatus-resource"></a>Recurso AsyncJobStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse recurso fornece informações sobre o progresso de um trabalho assíncrono.

A seguinte API chama recursos **AsyncJobStatus** de retorno:

* [Copiar item](../api/driveitem-copy.md)

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade          | Tipo   | Descrição                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| **percentageComplete** | Duplo | Um valor entre 0 e 100 que indica o percentual concluído.                          |
| **status**             | String | Um valor de cadeia de caracteres que é mapeado para uma enumeração dos valores possíveis sobre o status do trabalho. |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->

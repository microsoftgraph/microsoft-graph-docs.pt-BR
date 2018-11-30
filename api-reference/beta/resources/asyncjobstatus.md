---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
ms.openlocfilehash: 9e0f95802f9f75930384ab1534bf4c519fd9cfeb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033472"
---
# <a name="asyncjobstatus-resource"></a>Recurso AsyncJobStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->

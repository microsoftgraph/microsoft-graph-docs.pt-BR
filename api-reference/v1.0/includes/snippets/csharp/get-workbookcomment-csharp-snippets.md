---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5df2552d6292d316f2d615dfa3c675abb5e88b1f
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41497348"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookComment = await graphClient.Drive.Items["{id}"].Workbook.Comments["{id}"]
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f8380ff93709a01eec793180b5064684a36e935
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468616"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableSort = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Request()
    .GetAsync();

```
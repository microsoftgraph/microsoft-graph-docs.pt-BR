---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7dfbc7eccffb58b85c06b94ce4941992dff8a32
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .Range()
    .Request()
    .GetAsync();

```
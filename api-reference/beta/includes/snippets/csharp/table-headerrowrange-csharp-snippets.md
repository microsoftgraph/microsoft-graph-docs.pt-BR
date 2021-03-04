---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 589a7e179a9256c4630e990a8fd0d2e903bb77e4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .HeaderRowRange()
    .Request()
    .GetAsync();

```
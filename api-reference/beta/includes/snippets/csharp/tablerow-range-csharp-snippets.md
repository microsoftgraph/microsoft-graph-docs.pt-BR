---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1ea6558a7c7f204e260fd6b1291edc17c47c4fd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440583"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"]
    .Range()
    .Request()
    .GetAsync();

```
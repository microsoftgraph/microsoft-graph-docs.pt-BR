---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0455d0183d6e559b96f7cbfde42bf20a22d8e652
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442439"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Request()
    .GetAsync();

```
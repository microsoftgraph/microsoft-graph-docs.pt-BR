---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0455d0183d6e559b96f7cbfde42bf20a22d8e652
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874850"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Request()
    .GetAsync();

```
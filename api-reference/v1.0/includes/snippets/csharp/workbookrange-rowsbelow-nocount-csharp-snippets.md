---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbabb582c3f6826be8a69ef9363117d654818939
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow()
    .Request()
    .GetAsync();

```
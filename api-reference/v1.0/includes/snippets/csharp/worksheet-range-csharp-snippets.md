---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea7e7435b09584e0024e5a7f9012656cdd5ed1f0168fdb39c69bf379002ff7ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("A1:B2")
    .Request()
    .GetAsync();

```
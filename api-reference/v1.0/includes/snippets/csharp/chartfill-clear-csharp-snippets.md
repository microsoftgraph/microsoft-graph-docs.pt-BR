---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7ee19689e535e492c1dacac37bddd0c032c093668decbecbec68a403d4156f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```
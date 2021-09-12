---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4609692f06a83db9a92dfd40a002586b0367afa61f7a6ac9856a66d2209dd14b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format
    .AutofitRows()
    .Request()
    .PostAsync();

```
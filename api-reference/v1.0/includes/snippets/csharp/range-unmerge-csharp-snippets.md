---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd6f90932ee02f83999141184fbcd4df0ba793891173ba20a464059147f36d11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Unmerge()
    .Request()
    .PostAsync();

```
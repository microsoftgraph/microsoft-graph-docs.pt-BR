---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d642c997e7f3298851ff71e9605b2f816da38aea25cab289bb6cb5b841f30038
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook
    .RefreshSession()
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```
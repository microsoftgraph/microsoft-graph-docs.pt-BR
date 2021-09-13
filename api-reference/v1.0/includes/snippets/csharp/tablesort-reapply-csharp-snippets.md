---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa2ad9f3175b3b96dc5f5e81f7b46736e1bffafaf423d2324285fed8853fe02c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Reapply()
    .Request()
    .PostAsync();

```
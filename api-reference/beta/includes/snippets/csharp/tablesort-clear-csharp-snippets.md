---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9d614c324a2307240a864fa534c58d957ee0e55
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Clear()
    .Request()
    .PostAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 951e220998afe9482b9b1df1908f9b0aacf10ed9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"].Content
    .Request()
    .GetAsync();

```
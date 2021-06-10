---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1dbff0e0c971c7160ca3c57d54ef54ca8f0d671
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getPrinterArchivedPrintJobs = await graphClient.Print.Reports
    .GetPrinterArchivedPrintJobs("016b5565-3bbf-4067-b9ff-4d68167eb1a6","2021-05-24","2021-05-25")
    .Request()
    .GetAsync();

```
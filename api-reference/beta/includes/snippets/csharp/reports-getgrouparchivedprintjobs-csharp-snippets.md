---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4dc5bfb2a190887ababf58eb1dd8a6575dedac12df7897d9ba82fddcccf01f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getGroupArchivedPrintJobs = await graphClient.Print.Reports
    .GetGroupArchivedPrintJobs("016b5565-3bbf-4067-b9ff-4d68167eb1a6","2021-05-24","2021-05-25")
    .Request()
    .GetAsync();

```
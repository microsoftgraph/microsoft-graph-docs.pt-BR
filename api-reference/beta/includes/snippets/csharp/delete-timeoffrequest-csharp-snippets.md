---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4af07aa548115ea66030bd413030df4d2d45fed
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.TimeOffRequests["{timeOffRequestId}"]
    .Request()
    .DeleteAsync();

```
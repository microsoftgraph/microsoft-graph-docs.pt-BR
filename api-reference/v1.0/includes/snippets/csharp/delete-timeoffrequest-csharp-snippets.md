---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adeb87ffea85538595cf7566d15351b746bb9b031704e078b16c048ce3ca3e44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Request()
    .DeleteAsync();

```
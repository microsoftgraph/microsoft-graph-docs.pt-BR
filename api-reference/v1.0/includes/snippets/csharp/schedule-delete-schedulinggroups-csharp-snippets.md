---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9924c8f78cb85dad0c043f243ecce715052286f1623a493faf9e5bd8a7e734aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.SchedulingGroups["{schedulingGroup-id}"]
    .Request()
    .DeleteAsync();

```
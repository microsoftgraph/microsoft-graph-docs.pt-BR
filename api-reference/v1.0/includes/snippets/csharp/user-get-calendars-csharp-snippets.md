---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96efbd55b22ff3f8df05c7d4b3067aef2dc335f34354ed5528bb43bc6922d2f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.Calendars
    .Request()
    .GetAsync();

```
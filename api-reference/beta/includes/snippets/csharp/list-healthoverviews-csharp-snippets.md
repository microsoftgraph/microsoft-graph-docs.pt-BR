---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7790523f28251201bc3ee5df843a62f9fd0b1a9570bd23c9d1d518ec3a43b4be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var healthOverviews = await graphClient.Admin.ServiceAnnouncement.HealthOverviews
    .Request()
    .GetAsync();

```
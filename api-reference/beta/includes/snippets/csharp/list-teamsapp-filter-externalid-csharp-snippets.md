---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17c909a7aedf06228a5dd80dcdde1c20ee3469873d00171508540607e6e71506
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .GetAsync();

```
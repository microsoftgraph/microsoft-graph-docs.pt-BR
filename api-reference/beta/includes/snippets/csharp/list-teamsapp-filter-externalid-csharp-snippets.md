---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 129dd4b9277f90ad0b07b35ea9a500673eacf2f7
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d625703b67cddf119170bf22e8e9c8143a269a0b
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("distributionMethod eq 'organization'")
    .GetAsync();

```
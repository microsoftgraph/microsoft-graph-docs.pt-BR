---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0941c3ed757b79ddfeb0f6ef6045487049e1710658c83f68df4c7f7df7424106
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273082"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = await graphClient.Teams["{team-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Request()
    .GetAsync();

```
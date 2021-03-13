---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd1388bcdb218ba44c297ea1406d39dab28c9145
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = await graphClient.Teams["{team-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3a8d57fed6293c68af576e1ef6c5de36ac332b7bc697df2f2e9f08aaeeba6a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376643"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```
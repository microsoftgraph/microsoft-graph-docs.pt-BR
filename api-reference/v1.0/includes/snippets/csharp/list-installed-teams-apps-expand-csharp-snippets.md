---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cb6728a68f1721737fe9906d65500b37bf0d83f
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["6903fa93-605b-43ef-920e-77c4729f8258"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```
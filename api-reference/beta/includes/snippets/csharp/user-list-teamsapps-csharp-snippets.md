---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c69c7edb14f2f59b3db3ca2d426d783b683253d8
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["{id}"].Teamwork.InstalledApps
    .Request()
    .GetAsync();

```
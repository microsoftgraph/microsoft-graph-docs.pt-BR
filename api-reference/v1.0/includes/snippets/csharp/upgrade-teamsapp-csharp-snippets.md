---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 795b7e4079c9c4698982300b81957a592a99c328
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].InstalledApps["{id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```
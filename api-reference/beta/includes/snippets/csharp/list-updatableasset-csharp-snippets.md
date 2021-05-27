---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf34e504c64be9f586c2ef8634e43cc6f4876cee
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience.Members
    .Request()
    .GetAsync();

```
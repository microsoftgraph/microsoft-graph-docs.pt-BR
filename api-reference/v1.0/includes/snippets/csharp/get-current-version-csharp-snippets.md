---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ded05bdb5a8cb9560e28aba423006fc62ce5bdf3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItemVersion = await graphClient.Me.Drive.Items["{driveItem-id}"].Versions["{driveItemVersion-id}"]
    .Request()
    .GetAsync();

```
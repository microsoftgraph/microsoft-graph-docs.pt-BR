---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f568aede427220844da45a34677832238a04e1b4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var incomingChannels = await graphClient.Teams["{team-id}"].IncomingChannels
    .Request()
    .GetAsync();

```
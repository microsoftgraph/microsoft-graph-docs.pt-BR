---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6119ab7d1e4282e8c1bab52e41f12abc912b00b7fe3d430f03afdd5d0546fb4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals
    .Request()
    .GetAsync();

```
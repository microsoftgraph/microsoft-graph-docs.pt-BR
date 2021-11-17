---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab625cda64991eecfdec0de8a131a9dfe5682467cb4d2f2d0949995f281a3821
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = await graphClient.Identity.UserFlows["{identityUserFlow-id}"]
    .Request()
    .GetAsync();

```
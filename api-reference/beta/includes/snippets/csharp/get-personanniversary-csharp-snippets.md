---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d708df91372bb8df47cc7b37857580ac1c51a4ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = await graphClient.Me.Profile.Anniversaries["{personAnnualEvent-id}"]
    .Request()
    .GetAsync();

```
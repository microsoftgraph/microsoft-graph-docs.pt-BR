---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a08a1ac192c2df11d432f3f103eaa8667b3a89a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = await graphClient.Teams["{team-id}"]
    .Request()
    .GetAsync();

```
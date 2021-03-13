---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a7517a3137de6bad89d97faa4b83595e35da79f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShifts = await graphClient.Teams["{team-id}"].Schedule.OpenShifts
    .Request()
    .GetAsync();

```
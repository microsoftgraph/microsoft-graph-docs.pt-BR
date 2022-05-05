---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0c5ccebdba9f7eb3bb4cb9588ca46b39eaace20
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var associatedTeams = await graphClient.Me.Teamwork.AssociatedTeams
    .Request()
    .GetAsync();

```
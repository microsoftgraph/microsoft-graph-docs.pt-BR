---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74feb3e07eefdfa63b14f7cd644863b352828ca3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["{activity-id}"]
    .Request()
    .DeleteAsync();

```
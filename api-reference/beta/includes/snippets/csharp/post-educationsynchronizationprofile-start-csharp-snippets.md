---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12dc129e35fc86d0a802c06c7e2a9fee8ae49a15
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Start()
    .Request()
    .PostAsync();

```
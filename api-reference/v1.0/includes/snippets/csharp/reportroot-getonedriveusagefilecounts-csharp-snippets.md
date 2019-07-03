---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac0a2aeb9973d9d31205cb7cd61a0c5b6c191e25
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```
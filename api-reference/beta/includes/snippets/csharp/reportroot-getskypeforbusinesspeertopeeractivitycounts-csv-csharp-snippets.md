---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55125a284f587db3f5706bac9cc0a83f34d887b0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityCounts = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityCounts('D7')
    .Request()
    .GetAsync();

```
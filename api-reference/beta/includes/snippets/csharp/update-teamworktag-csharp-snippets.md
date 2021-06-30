---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9901334a7e6fe90d32b11699d34bd0190498168
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210099"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTag = new TeamworkTag
{
    DisplayName = "Finance"
};

await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"]
    .Request()
    .UpdateAsync(teamworkTag);

```
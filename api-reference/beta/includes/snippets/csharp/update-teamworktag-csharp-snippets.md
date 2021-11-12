---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a4e86ab23e30a809dee37d5baa2b32b2b5191a124aaa00f329eb2b78fd2e89b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101936"
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
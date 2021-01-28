---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19692413416f879460673702b657cfe5acd86b74
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{school-id}"].Users["{user-id}"]
    .Request()
    .DeleteAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54fc34ec937d872a4328eba95e987f744c278edd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
    .Request()
    .DeleteAsync();

```
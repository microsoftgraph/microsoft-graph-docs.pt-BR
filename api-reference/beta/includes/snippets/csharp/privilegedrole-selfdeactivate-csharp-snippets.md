---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce6f340975b82ff891deedc9b7277265d93ae34923e5b421a4fa658d60efad48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159202"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoles["{privilegedRole-id}"]
    .SelfDeactivate()
    .Request()
    .PostAsync();

```
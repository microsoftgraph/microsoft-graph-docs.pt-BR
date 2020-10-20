---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6aa7ae895baade00992d77d1abe0efb7721deb4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620197"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSummary = await graphClient.PrivilegedRoles["{id}"].Summary
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eabe384e45cdbb35eaeb67e506fbabde5d4861c5a04cb31f2cf9ee4adfffa057
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
    .Request()
    .Filter("isElevated eq true")
    .GetAsync();

```
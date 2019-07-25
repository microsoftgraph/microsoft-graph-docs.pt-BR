---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2be210960b5584ff9fa182850d5d03e63f2dab89
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```
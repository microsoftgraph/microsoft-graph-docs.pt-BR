---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b30ede5875ff2e10b3d9bf4dbe29345211243e5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706440"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domainNameReferences = await graphClient.Domains["contoso.com"].DomainNameReferences
    .Request()
    .GetAsync();

```
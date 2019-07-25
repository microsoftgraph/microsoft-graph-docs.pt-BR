---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df033299fdf749885fa325181e5184f66d0d740a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Me
    .Request()
    .GetAsync();

```
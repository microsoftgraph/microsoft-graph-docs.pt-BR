---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9a82cdb740df7bb2e5713de9fe480a88c257363
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715080"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users.Delta()
    .Request()
    .GetAsync();

```
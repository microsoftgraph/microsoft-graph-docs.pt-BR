---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9a82cdb740df7bb2e5713de9fe480a88c257363
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users.Delta()
    .Request()
    .GetAsync();

```
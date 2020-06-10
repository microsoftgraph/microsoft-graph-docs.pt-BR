---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86de4386c0fd94466aaf71803244193c1d0ae1b4
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Directory.DeletedItems
    .Request()
    .GetAsync();

```
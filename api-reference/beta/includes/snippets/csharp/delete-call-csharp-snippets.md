---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 881ec7bac57269dbf90029c04bc7ea76988cf56c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708997"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"]
    .Request()
    .DeleteAsync();

```
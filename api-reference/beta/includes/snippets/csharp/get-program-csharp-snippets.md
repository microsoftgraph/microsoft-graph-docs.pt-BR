---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 090b9ad328a4fcf3653448ce3a69330a28a6a1cd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programs = await graphClient.Programs
    .Request()
    .GetAsync();

```
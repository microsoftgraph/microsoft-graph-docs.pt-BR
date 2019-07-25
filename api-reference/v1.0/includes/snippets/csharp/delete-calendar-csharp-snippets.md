---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 168d963ab77e81f46725e5846653c8be2c6e8a12
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Calendar
    .Request()
    .DeleteAsync();

```
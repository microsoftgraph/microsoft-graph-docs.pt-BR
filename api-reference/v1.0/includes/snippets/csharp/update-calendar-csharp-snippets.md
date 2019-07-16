---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0aab50285e7b65a8abc36358cc839276ff0f0f9b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Social events"
};

await graphClient.Me.Calendar
    .Request()
    .UpdateAsync(calendar);

```
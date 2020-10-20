---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79f310d7fd77e2896bb03a855b221e835952b27d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .GetAsync();

```
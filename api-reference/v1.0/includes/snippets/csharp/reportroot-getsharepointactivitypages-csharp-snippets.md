---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 266c2447f5d1b2e24fa267c8687d430638f6eca0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 189aabf7420f5dbc5c03fcffbc5e69bb78fc6001
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Me.Classes
    .Request()
    .GetAsync();

```
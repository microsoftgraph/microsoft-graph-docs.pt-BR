---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76a687d6c802325a064108e81c253f738c44e6d2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Settings
    .Request()
    .GetAsync();

```
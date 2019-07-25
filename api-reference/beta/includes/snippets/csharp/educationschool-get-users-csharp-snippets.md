---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae3c97d78268a5fb75bdb2342de226d9d8d820cd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Schools["10002"].Users
    .Request()
    .GetAsync();

```
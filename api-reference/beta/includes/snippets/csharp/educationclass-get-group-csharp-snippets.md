---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d262498121392822ca43f07c489062bd2c729c8f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Education.Classes["{educationClass-id}"].Group
    .Request()
    .GetAsync();

```
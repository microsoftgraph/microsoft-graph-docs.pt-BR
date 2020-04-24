---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6f7e45960962e9e633ede3ec0571542c57d733e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var longRunningOperation = await graphClient.Users["{id}"].Authentication.Operations["{id}"]
    .Request()
    .GetAsync();

```
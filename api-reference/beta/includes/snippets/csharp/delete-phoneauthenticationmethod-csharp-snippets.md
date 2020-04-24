---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0b77278164337062d6a0e09d45e83223ed01026
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Authentication.PhoneMethods["3179e48a-750b-4051-897c-87b9720928f7"]
    .Request()
    .DeleteAsync();

```
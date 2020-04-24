---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29422f05940f6e1459e8355e747d18c0edb252bf
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].Authentication.PasswordMethods["{id}"]
    .ResetPassword(null,null)
    .Request()
    .PostAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1370283501ebcc097fedde08652df9d684a1fc18
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944625"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowLanguageConfiguration = new UserFlowLanguageConfiguration
{
    Id = "es-ES",
    IsEnabled = true
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"]
    .Request()
    .PutAsync(userFlowLanguageConfiguration);

```
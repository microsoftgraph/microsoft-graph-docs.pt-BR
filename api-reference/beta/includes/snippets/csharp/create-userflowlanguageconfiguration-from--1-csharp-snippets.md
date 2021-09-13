---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e40d719a6f6f7fd6cd78393760e7892b6601226cee6a19a1894d512c9ba2009
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213862"
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
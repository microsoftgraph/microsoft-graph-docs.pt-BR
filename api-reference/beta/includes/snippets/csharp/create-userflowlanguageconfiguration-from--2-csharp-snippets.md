---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7db149ca14f65434baecb11f5d822d3c1417f1a5f1eb659beff6b619e9623236
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowLanguageConfiguration = new UserFlowLanguageConfiguration
{
    IsEnabled = false
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"]
    .Request()
    .PutAsync(userFlowLanguageConfiguration);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a1516172db8f7e72c19569ffcaf7f2892a5f76057bd0ce670f9239a6a23fef0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserFlowIdentityProviders
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3296889bfc147f99a652df07eae97bf140b948caab8b7f29f22ceea05e2cfe5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"]
    .Request()
    .DeleteAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44af0f3f6926f69652a07fce10b5262d88bd291c5f54e675918a82728426a1e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213881"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages
    .Request()
    .Filter("isEnabled eq true")
    .GetAsync();

```
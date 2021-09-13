---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6b4b23994160391acf21816b1d5465ee443b8f2ee182b4bc0b3f31fddf7b2e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"]
    .Request()
    .GetAsync();

```
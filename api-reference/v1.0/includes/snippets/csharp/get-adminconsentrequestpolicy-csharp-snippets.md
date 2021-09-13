---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e16101da333615508efe48765dcd5eae7760929ad14126125fd23fb15d9a2d89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var adminConsentRequestPolicy = await graphClient.Policies.AdminConsentRequestPolicy
    .Request()
    .GetAsync();

```
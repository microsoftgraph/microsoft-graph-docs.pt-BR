---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5af64408d8a330a4ade489b8fad8cf0dd02edbdf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].Languages
    .Request()
    .GetAsync();

```
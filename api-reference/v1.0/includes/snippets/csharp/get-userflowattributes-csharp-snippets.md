---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 821d864253966b83ee5c3464024d878c7840d54e60ee056fde2c79e04ff9250a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttribute = await graphClient.Identity.UserFlowAttributes["{identityUserFlowAttribute-id}"]
    .Request()
    .GetAsync();

```
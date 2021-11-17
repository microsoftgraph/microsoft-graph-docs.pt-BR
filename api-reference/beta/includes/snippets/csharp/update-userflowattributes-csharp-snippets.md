---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83715ac60222cfbce091176a18827ed1f3377e9cfe335d79659bbcf0aeae26d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttribute = new IdentityUserFlowAttribute
{
    Description = "Your new hobby"
};

await graphClient.Identity.UserFlowAttributes["{identityUserFlowAttribute-id}"]
    .Request()
    .UpdateAsync(identityUserFlowAttribute);

```
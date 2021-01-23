---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12fe072103df19691b481da88fcabba24de37577
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["B2C_1_CustomerSignUp"].IdentityProviders["Facebook-OAUTH"].Reference
    .Request()
    .DeleteAsync();

```
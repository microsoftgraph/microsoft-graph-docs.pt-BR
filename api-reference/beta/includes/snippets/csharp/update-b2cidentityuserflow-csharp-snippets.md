---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1f89095247258513d533f26d64519683e7e498b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    IsLanguageCustomizationEnabled = true,
    DefaultLanguageTag = "en"
};

await graphClient.Identity.B2cUserFlows["B2C_1_CustomerSignUp"]
    .Request()
    .UpdateAsync(b2cIdentityUserFlow);

```
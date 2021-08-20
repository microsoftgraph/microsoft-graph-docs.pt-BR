---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2e9bae6018ed2a163ddc403d4936cb96a4274a5dd92e847ee8a938dbe438c0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new IdentityProviderBase
{
    DisplayName = "Apple"
};

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .UpdateAsync(identityProviderBase);

```
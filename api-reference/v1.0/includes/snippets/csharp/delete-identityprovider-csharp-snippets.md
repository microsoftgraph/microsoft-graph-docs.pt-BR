---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4777f50454560502e71079a8c2a18aa6b7ca6f6965f130ba27c6318feb53dc30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .DeleteAsync();

```
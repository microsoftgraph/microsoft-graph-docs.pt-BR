---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71c0334e9824a1ed5e396468d39f7e30bb175505a673ebc100e318d335f90bbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Authentication.PhoneMethods["{phoneAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```
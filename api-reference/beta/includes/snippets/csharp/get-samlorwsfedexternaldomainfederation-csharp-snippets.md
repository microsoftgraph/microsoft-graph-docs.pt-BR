---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d88665dcdf5dcabba53e3dbe08079b719e53116
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var samlOrWsFedExternalDomainFederation = await graphClient.Directory.FederationConfigurations
    .Request()
    .Filter("domains/any(x: x/id eq 'contoso.com')")
    .GetAsync();

```
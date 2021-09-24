---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0068a139c0834d663d58bfb8b6ccd84677f333dd
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508587"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var samlOrWsFedExternalDomainFederation = await graphClient.Directory.FederationConfigurations
    .Request()
    .GetAsync();

```
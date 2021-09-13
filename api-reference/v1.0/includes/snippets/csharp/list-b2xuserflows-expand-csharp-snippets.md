---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4bdceecaeb757c76fdc051a6b596af0f34ebaf6bea0edaaa9115e6b7b56155f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows
    .Request()
    .Expand("identityProviders")
    .GetAsync();

```
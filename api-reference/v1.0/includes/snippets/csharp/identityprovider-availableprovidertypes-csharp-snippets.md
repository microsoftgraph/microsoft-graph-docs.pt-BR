---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4af41a86dbbf74ed743a82b68afef62627665fdfdc595368c1aaaa224b74a951
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availableProviderTypes = await graphClient.IdentityProviders
    .AvailableProviderTypes()
    .Request()
    .GetAsync();

```
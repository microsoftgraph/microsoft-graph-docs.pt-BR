---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 432e2608e1dd6d3efaf87f55ffc9d11bc01e277e21ff490d407bc20752524791
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .GetAsync();

```
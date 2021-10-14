---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 883f44b55c28e1b6af550a7638146f3e6c4d970cb86954659467c2229c8a1ac2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Contacts["{orgContact-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```
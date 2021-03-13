---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38e09c248ee3bfa50bf0a5073bff93c44b2c4d5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Contacts["{orgContact-id}"].MemberOf
    .Request()
    .GetAsync();

```
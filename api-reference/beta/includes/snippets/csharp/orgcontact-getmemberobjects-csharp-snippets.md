---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95788615fcf8d03db3fce6fd106b600811fe386b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Contacts["{orgContact-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```
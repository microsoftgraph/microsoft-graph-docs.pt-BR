---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 224ca09366572c573c672b9e12cfb6d6ba3d7407
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Users["{user-id}"].MemberOf
    .Request()
    .GetAsync();

```
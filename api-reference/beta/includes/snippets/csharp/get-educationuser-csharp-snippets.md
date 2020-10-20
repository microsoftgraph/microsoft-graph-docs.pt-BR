---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3e97f44dcc26a0537b483d10aec5d702887f47c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619364"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["13012"]
    .Request()
    .GetAsync();

```
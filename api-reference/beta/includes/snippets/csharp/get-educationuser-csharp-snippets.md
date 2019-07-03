---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3e97f44dcc26a0537b483d10aec5d702887f47c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["13012"]
    .Request()
    .GetAsync();

```
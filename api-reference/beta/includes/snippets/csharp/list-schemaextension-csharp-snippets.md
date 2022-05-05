---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbd4103b7c53d8d8cdc68cb062659158c47d059e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select("ext55gb1l09_msLearnCourses")
    .GetAsync();

```
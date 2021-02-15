---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2fcd819bde2baeaa0ae468ff27154ce7e15e8d4
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50243078"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Schools["{school-id}"].Classes
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4570033211a0a5311542182c36f94eccb035577d60902440f55b3bd55786f0ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var people = await graphClient.Me.People
    .Request()
    .GetAsync();

```
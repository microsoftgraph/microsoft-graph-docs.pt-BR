---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6311856968c5b3f1d52e98ff6dcd838d68f1ecb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me
    .FindRooms('Building2Rooms@contoso.onmicrosoft.com')
    .Request()
    .GetAsync();

```
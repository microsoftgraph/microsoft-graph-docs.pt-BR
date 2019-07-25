---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a6e93d95b4955725b680778bd8eb46626bc3dad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867744"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRoomLists = await graphClient.Me
    .FindRoomLists()
    .Request()
    .GetAsync();

```
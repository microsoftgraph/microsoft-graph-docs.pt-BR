---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6ac0e2391255a63614ff7948d9f6c1b7a83aefa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473754"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusinesses = await graphClient.BookingBusinesses
    .Request()
    .GetAsync();

```
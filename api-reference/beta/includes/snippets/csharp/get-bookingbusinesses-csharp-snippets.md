---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6ac0e2391255a63614ff7948d9f6c1b7a83aefa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusinesses = await graphClient.BookingBusinesses
    .Request()
    .GetAsync();

```
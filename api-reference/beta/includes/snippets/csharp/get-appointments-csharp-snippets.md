---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06aad25fbfedd71168c86cb8f33e9898591e1db5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appointments = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Appointments
    .Request()
    .GetAsync();

```
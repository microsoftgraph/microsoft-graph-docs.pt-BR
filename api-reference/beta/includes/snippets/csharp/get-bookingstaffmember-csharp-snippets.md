---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50afd3dedfc04e2eb0fec437349934bcd82a4477
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792272"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers["{bookingStaffMember-id}"]
    .Request()
    .GetAsync();

```
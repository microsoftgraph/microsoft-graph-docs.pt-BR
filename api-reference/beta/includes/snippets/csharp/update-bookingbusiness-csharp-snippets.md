---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 094f85528995fc75d2385504cf37c4ffc27b0028
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = new BookingBusiness
{
    Email = "admin@fabrikam.com",
    SchedulingPolicy = new BookingSchedulingPolicy
    {
        TimeSlotInterval = new Duration("PT60M"),
        MinimumLeadTime = new Duration("P1D"),
        MaximumAdvance = new Duration("P30D"),
        SendConfirmationsToOwner = true,
        AllowStaffSelection = true
    }
};

await graphClient.BookingBusinesses["fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .UpdateAsync(bookingBusiness);

```
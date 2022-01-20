---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83d73a181a9a4e678aa270f0889fbb69f84e8312
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094579"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    DisplayName = "Adele"
    EmailAddress = "adele@relecloud.com"
}

Update-MgBookingBusinessCustomer -BookingBusinessId $bookingBusinessId -BookingCustomerId $bookingCustomerId -BodyParameter $params

```
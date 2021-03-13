---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a53e412ae326afb01874cb5db7bdcee60823f4fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Appointments["{bookingAppointment-id}"]
    .Cancel(cancellationMessage)
    .Request()
    .PostAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aecd5388fe82e457fc395156cc9518ed4ac050517826de582720af065cb7c988
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Appointments["{bookingAppointment-id}"]
    .Cancel(cancellationMessage)
    .Request()
    .PostAsync();

```
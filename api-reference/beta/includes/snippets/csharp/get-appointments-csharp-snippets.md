---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae1cc49effde3e18ef124eb3df2836fb18a57766aa32272b0389ec31561ae144
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101816"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appointments = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Appointments
    .Request()
    .GetAsync();

```
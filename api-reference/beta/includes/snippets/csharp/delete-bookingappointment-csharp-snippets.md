---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7853e03d24df86cfd687501428c58dded06328650bf350e0ed9745505486756
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Appointments["{bookingAppointment-id}"]
    .Request()
    .DeleteAsync();

```
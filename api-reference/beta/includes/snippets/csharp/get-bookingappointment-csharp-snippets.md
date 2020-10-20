---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a982c89118276eb60326cd8f4236a6271db8604f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingAppointment = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKnAAA="]
    .Request()
    .GetAsync();

```
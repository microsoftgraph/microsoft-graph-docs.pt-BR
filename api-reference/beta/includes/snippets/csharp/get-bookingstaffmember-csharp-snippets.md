---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f25e4abdc267e2625481c248a9372aed2b436f2c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["71d64d0e-7225-49b6-b0b1-070d476cda51"]
    .Request()
    .GetAsync();

```
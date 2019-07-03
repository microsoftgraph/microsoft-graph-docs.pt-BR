---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d53f3fafdda4da97e14e9a2e4ca84a2527a67895
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499089"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var staffMembers = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers
    .Request()
    .GetAsync();

```
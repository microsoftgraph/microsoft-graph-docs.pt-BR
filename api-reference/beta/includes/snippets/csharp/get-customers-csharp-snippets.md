---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 872d736e63ce4e9119ef4cb49eb66342ebde92b5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customers = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers
    .Request()
    .GetAsync();

```
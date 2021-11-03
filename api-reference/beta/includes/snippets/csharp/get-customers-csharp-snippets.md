---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67c9e4d534259ab8abe4205531803c385285b2cfe8373c6f9d18ca775fab476b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customers = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers
    .Request()
    .GetAsync();

```
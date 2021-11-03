---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b50a4e02d01eebcbecf8b735450d6a427cd11553bdde4575d0539abebe2076a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services["{bookingService-id}"]
    .Request()
    .GetAsync();

```
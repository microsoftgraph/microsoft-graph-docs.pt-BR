---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f148e3cfda96c00e82a2ac0627b23534986ba5f8aac9b9bcfa073b4ed2398eb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Publish()
    .Request()
    .PostAsync();

```
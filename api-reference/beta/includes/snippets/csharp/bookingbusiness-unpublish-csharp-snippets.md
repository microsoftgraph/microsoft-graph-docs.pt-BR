---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1f516c0d6542006531a9cda7ff08c8f4c9d03df3fd7131623c3519505a2a23d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Unpublish()
    .Request()
    .PostAsync();

```
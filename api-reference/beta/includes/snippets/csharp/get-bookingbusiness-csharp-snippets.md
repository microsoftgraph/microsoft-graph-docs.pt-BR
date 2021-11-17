---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcef44851244ddead9860032d1dbae38df0811ed4ea6cbea62a1dd8aea814d0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157642"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Request()
    .GetAsync();

```
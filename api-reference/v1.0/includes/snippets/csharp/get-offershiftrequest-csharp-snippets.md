---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a406f986a87498617eea996b1ed141fbd96b310e
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequests = await graphClient.Teams["{teamId}"].Schedule.OfferShiftRequests
    .Request()
    .GetAsync();

```
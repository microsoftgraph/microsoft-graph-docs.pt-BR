---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 344ac93cefa49cc17101552254c6a45bbe0a2f34
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowAttributes = await graphClient.Identity.UserFlowAttributes
    .Request()
    .GetAsync();

```
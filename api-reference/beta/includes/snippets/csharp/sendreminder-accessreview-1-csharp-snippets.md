---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40445c76aebf5a6a818af43fa3e9396f273a9894a35c2d050e03b014ae276376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .SendReminder()
    .Request()
    .PostAsync();

```
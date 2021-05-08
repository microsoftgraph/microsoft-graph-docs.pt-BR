---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98a1011c3f6643718b4f53d197343f277682ac46
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240620"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewPolicy = new AccessReviewPolicy
{
    IsGroupOwnerManagementEnabled = true
};

await graphClient.Policies.AccessReviewPolicy
    .Request()
    .UpdateAsync(accessReviewPolicy);

```
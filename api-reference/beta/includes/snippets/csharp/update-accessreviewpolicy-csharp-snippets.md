---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 018a60aec3f8fdec06d88aee7003c1ba43e5c6db3be1bf83f0b4687d926788ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898157"
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
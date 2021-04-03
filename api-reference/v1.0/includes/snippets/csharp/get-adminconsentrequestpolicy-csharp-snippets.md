---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55cece7bdea29ba88c0a3c663bb8b4a42c0359e0
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var adminConsentRequestPolicy = await graphClient.Policies.AdminConsentRequestPolicy
    .Request()
    .GetAsync();

```
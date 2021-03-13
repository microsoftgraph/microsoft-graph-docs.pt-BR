---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f65129215170629c7e214ce20cd9513c84b7e1b6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807138"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration["{certificateBasedAuthConfiguration-id}"]
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 658cce317d69187fcb913c0a960a80ec3b871af3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration["{certificateBasedAuthConfiguration-id}"]
    .Request()
    .DeleteAsync();

```
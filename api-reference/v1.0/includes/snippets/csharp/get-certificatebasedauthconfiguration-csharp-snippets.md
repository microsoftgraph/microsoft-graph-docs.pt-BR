---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d562d8d01a719e0e362f55a833f154297c72a75b
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration["{id}"]
    .Request()
    .GetAsync();

```
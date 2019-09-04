---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1cfaba23b71210e0b9772724fc579fcbdd7d458
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration["{id}"]
    .Request()
    .DeleteAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb143d00ead236726b37b1e8f2d29d4106a1d476
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["contoso.com"]
    .Request()
    .DeleteAsync();

```
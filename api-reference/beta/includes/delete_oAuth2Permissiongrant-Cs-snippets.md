---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4704bcf05f8ec173451f0b4d7d66dbef23b7be35
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OAuth2Permissiongrants["{id}"]
    .Request()
    .DeleteAsync();

```
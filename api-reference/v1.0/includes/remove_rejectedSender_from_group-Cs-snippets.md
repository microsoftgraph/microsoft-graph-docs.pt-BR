---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c78c49b244444804fd0a11f17deac85e88835c57
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].RejectedSenders
    .Request()
    .DeleteAsync();

```
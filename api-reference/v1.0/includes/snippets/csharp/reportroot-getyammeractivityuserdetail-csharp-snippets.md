---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfb3d894266ff6fb2e2c92f84d8fafd5021450f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityUserDetail("D7")
    .Request()
    .GetAsync();

```
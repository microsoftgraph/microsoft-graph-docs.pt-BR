---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eff2cc816a2613a6fedc514d4e62386988b346ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityUserDetail("D7")
    .Request()
    .GetAsync();

```
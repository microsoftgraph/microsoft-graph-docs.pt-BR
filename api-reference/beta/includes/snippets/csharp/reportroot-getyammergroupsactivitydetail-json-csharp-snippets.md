---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62179472bc4a44052f7ba94ee23c7f34c02e5d0a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityDetail = await graphClient.Reports
    .GetYammerGroupsActivityDetail("D7")
    .Request()
    .GetAsync();

```
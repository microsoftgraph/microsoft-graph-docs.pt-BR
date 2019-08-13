---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80a1fd1fbc43e14aa29f80caf960843b2788e1ff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityUserDetail = await graphClient.Reports
    .GetSkypeForBusinessActivityUserDetail("D7")
    .Request()
    .GetAsync();

```
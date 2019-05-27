---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f969b1c3a1bf20dfd59f6279e204d7eb0aae89d5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityUserDetail = await graphClient.Reports.GetSkypeForBusinessActivityUserDetail('D7')
    .Request()
    .GetAsync();

```
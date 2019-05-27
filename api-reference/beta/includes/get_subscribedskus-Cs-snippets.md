---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 948ed19e37dd3dfc2f4d902d017308261ec6f3e4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSkus = await graphClient.SubscribedSkus
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 839b860f5ac22250a3811413b929d91f8322386a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myRequests = await graphClient.PrivilegedApproval.MyRequests()
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9736f77673ba3109534e651a587fd3641c173d5b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .GetAsync();

```
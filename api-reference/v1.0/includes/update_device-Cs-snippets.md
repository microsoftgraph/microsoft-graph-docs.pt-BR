---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 848afda8c51daa2aac2656192ec8205f77a67635
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    AccountEnabled = false
};

await graphClient.Devices["{id}"]
    .Request()
    .UpdateAsync(device);

```
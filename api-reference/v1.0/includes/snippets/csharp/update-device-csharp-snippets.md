---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 848afda8c51daa2aac2656192ec8205f77a67635
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715925"
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
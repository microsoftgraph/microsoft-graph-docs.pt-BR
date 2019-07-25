---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8632a3ca72576a0eb24005cc6389c76e87279c1d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredDevices = await graphClient.Me.RegisteredDevices
    .Request()
    .GetAsync();

```
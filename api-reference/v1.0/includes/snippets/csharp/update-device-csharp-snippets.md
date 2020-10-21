---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 848afda8c51daa2aac2656192ec8205f77a67635
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607552"
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
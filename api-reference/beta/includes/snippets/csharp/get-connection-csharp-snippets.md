---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bf4e987c88d81b7c62df9f04c0ca2680804679f
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectionQuota = await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Quota
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 857c28ba01a84120f3baaa9c6c38f57bb6eaa64d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = await graphClient.Teams["{id}"]
    .Request()
    .GetAsync();

```
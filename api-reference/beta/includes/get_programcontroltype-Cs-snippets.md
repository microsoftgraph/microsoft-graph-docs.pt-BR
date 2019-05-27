---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22136ee585815c96be22ff1639227cda707e994c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControlTypes = await graphClient.ProgramControlTypes
    .Request()
    .GetAsync();

```
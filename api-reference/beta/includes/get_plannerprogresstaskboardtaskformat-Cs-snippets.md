---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad62b66f308c9da0b6ffad1ef297dba173839846
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["'id'"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```
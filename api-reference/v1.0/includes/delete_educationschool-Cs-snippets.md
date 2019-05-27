---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6fa6bcf334d47b90b18e90969d049bf19672292
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{school-id}"]
    .Request()
    .DeleteAsync();

```
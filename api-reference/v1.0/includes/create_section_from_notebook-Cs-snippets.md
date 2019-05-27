---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6aeda4f6b8388bb1ac4e9461dd6e95f534de7cf3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460078"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.Notebooks["{id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```
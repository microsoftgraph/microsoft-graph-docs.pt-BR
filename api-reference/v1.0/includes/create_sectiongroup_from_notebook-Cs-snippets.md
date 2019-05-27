---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b96fd4b1b44c6c3720dd9df3158f6b6aafc372fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.Notebooks["{id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```
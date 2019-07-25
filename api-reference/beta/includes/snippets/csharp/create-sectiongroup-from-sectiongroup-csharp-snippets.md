---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa65adfb7d6afde22365edb35ffd9fc680953629
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725447"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.SectionGroups["{id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```
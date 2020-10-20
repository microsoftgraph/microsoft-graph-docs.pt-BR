---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa65adfb7d6afde22365edb35ffd9fc680953629
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615039"
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
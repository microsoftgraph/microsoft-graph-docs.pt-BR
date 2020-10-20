---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b96fd4b1b44c6c3720dd9df3158f6b6aafc372fa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607493"
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
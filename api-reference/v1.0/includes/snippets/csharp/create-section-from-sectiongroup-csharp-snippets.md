---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2526f1bb7aa311714bd51162c3cf2312e15734d9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.SectionGroups["{id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2526f1bb7aa311714bd51162c3cf2312e15734d9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439614"
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
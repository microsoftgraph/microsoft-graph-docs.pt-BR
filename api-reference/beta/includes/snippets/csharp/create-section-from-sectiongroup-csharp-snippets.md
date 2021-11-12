---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49fc692b832990fa121f4d0e91be15315121cde60ddcec0bdb3916176c2dc627
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```
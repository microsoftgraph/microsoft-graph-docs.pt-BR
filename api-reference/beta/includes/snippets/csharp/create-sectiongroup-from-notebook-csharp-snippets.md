---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96f0ec87e58e8bae1ab1947da67954f6ff2e0537d60d26334100e458d46cd18e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.Notebooks["{notebook-id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```
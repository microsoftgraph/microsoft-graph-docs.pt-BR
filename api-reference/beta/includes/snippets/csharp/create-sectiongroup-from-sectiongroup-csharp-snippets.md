---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1cbe1935ec09159399fd8582bda76a8f5f0d3152cf686f32ea22ba6cb4c9357
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273397"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45e22591860e5985df8d24bfc0fd66a2bed958aa44911d620b29ce3c2fe58eff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = await graphClient.Me.Profile.EducationalActivities["{educationalActivity-id}"]
    .Request()
    .GetAsync();

```
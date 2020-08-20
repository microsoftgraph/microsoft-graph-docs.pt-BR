---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36b2ea5194361d77bc7ea663a6bd4d73b4dc8bcf
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.EducationalActivities["{id}"]
    .Request()
    .DeleteAsync();

```
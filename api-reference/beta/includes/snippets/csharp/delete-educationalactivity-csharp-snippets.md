---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 954cc12dd0bf03740bf2f36be743eaa342d91f0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.EducationalActivities["{educationalActivity-id}"]
    .Request()
    .DeleteAsync();

```
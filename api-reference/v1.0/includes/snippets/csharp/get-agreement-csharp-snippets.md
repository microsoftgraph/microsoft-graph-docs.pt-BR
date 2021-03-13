---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1b6e35f26f4e81051e96811a989042b6f3f48f1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .Expand("files")
    .GetAsync();

```
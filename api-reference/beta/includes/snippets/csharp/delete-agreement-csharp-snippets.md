---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebe46e9b3d2e0d7b99a1a5dd1a6ffefa00b04895
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .DeleteAsync();

```
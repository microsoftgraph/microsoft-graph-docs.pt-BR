---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7aba927be341392a3bcbc2afbad2621047d4139
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "Sample ToU display name",
    IsViewingBeforeAcceptanceRequired = true
};

await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .UpdateAsync(agreement);

```
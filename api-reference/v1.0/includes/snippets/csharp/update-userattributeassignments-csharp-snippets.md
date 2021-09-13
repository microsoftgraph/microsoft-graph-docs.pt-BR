---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eefae450996c80bf122dc6c8a58b40a3780af7a1604243670d8acf16a1a1ebe9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment
{
    UserInputType = IdentityUserFlowAttributeInputType.TextBox
};

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments["{identityUserFlowAttributeAssignment-id}"]
    .Request()
    .UpdateAsync(identityUserFlowAttributeAssignment);

```
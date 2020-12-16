---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f71749d80ee777232370777364b76260f8c4b572
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment
{
    UserInputType = IdentityUserFlowAttributeInputType.TextBox
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlowId}"].UserAttributeAssignments["{id}"]
    .Request()
    .UpdateAsync(identityUserFlowAttributeAssignment);

```
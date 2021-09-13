---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744f9e5902672d79a1c66da508d20a8dc0e80e2e35123fab438b96da4037813f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentOrder = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments
    .GetOrder()
    .Request()
    .GetAsync();

```
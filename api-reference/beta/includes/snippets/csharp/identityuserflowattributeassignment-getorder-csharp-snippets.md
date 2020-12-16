---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0037d172b23d9bc5643d4955cd9249588e5abc24
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentOrder = await graphClient.Identity.B2cUserFlows["{id}"].UserAttributeAssignments
    .GetOrder()
    .Request()
    .GetAsync();

```
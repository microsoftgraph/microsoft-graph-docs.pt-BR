---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44f0b614aa32ea29e871c74420a118af854e4bda60db207624d0d009988aa9f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentOrder = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments
    .GetOrder()
    .Request()
    .GetAsync();

```
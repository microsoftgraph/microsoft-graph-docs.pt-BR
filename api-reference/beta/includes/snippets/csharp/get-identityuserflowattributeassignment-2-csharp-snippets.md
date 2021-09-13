---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3782d4a2e78b1ef452534e2a889e4b2450213ac35019d8c18fb456ab2226582
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .GetAsync();

```
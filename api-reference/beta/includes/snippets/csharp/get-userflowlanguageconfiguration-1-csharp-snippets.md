---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92daea3cc7040d7bfa5c305480e9fd85d94336d8963af976332a675c0603e9f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages
    .Request()
    .GetAsync();

```
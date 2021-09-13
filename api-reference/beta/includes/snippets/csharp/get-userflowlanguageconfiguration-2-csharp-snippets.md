---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aff60ffad20ce5768ddddbda334a0db99439a10b2ef7fea35ec96689dc26bfba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].Languages
    .Request()
    .GetAsync();

```
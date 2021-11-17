---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02866ce934910929c9d5063dcd2fb27ea9ab275bba9df04234013f57758b0889
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"]
    .Request()
    .DeleteAsync();

```
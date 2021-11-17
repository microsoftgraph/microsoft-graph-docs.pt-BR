---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea6ddf08976cdb3c66a7503d5ba41a0808b0e7ba4201e28fe5cdf565e081ca59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"]
    .Request()
    .DeleteAsync();

```
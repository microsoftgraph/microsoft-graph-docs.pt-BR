---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc0f080022618ecb692bd12e5e6ca3df2d1410f1b7629d3051006e638ea84156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .Request()
    .GetAsync();

```
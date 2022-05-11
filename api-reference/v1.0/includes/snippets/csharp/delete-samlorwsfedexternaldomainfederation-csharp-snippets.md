---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1101baa35f39176c3f29b25d0f676221b86cd134
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.FederationConfigurations["{identityProviderBase-id}"]
    .Request()
    .DeleteAsync();

```
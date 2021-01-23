---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4d1461006a4e4ec8f4b0669c343b60b428b3378
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = await graphClient.IdentityProviders["{id}"]
    .Request()
    .GetAsync();

```
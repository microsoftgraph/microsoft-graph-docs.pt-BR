---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6460a1e294c275c6ec8540f6b293a741f761b3bd
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addresses = await graphClient.Me.Profile.Addresses
    .Request()
    .GetAsync();

```
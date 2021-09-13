---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbfe0bf197e57446e4f6f5c68db8ab94e74a5629
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59073841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availableProviderTypes = await graphClient.Identity.IdentityProviders
    .AvailableProviderTypes()
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd75b41a552511ea1c0a35464626e2e9e500b144
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Users["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df26514e6325d16e3f780705092c6da9a0e4c670
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61020367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var softwareOathAuthenticationMethod = await graphClient.Me.Authentication.SoftwareOathMethods["{softwareOathAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```
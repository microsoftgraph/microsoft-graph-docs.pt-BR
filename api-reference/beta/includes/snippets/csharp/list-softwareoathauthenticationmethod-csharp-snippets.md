---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52e576a8f567153e2980d163283a23284dc14b9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "60995199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var softwareOathMethods = await graphClient.Me.Authentication.SoftwareOathMethods
    .Request()
    .GetAsync();

```
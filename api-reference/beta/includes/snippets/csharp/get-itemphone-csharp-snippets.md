---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5489bb36330b53d55e505764c7f967bc6c50a6eb
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phones = await graphClient.Me.Profile.Phones
    .Request()
    .GetAsync();

```
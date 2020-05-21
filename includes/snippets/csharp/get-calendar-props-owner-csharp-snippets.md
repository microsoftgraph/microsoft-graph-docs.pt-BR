---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 205641f0c99a7c381084f596d72bffa9317fc21b
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendar
    .Request()
    .GetAsync();

```
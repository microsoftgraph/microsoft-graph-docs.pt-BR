---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be9e12937fdff58a4b6ff8987c906995feeb66ea
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Calendar.Events
    .Request()
    .Filter("startsWith(subject,'All')")
    .GetAsync();

```
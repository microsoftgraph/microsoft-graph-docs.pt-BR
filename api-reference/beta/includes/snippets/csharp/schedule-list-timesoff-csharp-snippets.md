---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3a70709de9f72029c41592820408400597444b8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timesOff = await graphClient.Teams["{teamId}"].Schedule.TimesOff
    .Request()
    .Filter("sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fdef774f7c92d8e53b7778f5a849caa0dff9f64e33601624b6ad141b9013e2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermissions = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendar.CalendarPermissions
    .Request()
    .GetAsync();

```
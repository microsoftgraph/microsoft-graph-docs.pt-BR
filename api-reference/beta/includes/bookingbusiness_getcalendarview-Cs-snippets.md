---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9982bd30522e4d5d849ac9164c84239c97ca4e7c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarView = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].CalendarView
    .Request()
    .GetAsync();

```
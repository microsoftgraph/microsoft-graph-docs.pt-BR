---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 980767b1ca413d4a4ac1cd8cff5fe5474f5dce29
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859666"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startdatetime", "{start_datetime}"));
requestOptions.add(new QueryOption("enddatetime", "{end_datetime}"));

IEventDeltaCollectionPage delta = graphClient.me().calendarView()
    .delta()
    .buildRequest( requestOptions )
    .get();

```
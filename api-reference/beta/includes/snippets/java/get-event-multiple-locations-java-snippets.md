---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0392ee58608082a354a456d967d359f3870f08bc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954868"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().events("AAMkADAGAADDdm4NAAA=")
    .buildRequest()
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location,locations")
    .get();

```
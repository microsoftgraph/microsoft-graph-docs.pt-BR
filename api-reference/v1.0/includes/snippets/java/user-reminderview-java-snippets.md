---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cc09fa56b150ddbacfd05d4b934818e2ce72121
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855165"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IReminderCollectionPage reminderView = graphClient.me()
    .reminderView('2017-06-05T10:00:00.0000000','2017-06-11T11:00:00.0000000')
    .buildRequest()
    .get();

```
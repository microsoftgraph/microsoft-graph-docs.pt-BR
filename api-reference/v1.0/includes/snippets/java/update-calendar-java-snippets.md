---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 992024b3d5ae71be020e6bae6e24cde5684e05f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882390"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Social events";

graphClient.me().calendar()
    .buildRequest()
    .patch(calendar);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc2cc89c5cc46199659ca346f18428e604b67d89
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859742"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Cancelling for this week due to all hands";

graphClient.me().events("{id}")
    .cancel(comment)
    .buildRequest()
    .post();

```
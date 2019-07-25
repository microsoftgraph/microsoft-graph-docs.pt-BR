---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23d878eb679fd3111e7f12fd903fe171270eb1b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855516"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.agreements("'id'")
    .buildRequest()
    .delete();

```
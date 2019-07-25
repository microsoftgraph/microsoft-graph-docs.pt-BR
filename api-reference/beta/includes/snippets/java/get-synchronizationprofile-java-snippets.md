---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edbea9bc3db7ff1d42cb23060a1811cb74a3400a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860077"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .buildRequest()
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2305392e06986fd7d87252ff81871768dc52fd74
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892442"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserCounts('D7')
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c51d7b967d5aaf5a36bafa2db606434b03d8677b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893988"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActiveUserDetail('D7')
    .buildRequest()
    .get();

```
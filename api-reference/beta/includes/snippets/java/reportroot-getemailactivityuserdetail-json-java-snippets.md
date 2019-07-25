---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5f39907a1b0e222ebd36953725356865ef135f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873978"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailActivityUserDetailCollectionPage getEmailActivityUserDetail = graphClient.reports()
    .getEmailActivityUserDetail('D7')
    .buildRequest()
    .get();

```
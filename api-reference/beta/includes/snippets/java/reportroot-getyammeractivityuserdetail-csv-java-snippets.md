---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0624275040f432d014c1046c7b46f177d8ca65f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871538"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivityUserDetailCollectionPage getYammerActivityUserDetail = graphClient.reports()
    .getYammerActivityUserDetail('D7')
    .buildRequest()
    .get();

```